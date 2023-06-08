# Comparing `tmp/kgraph-1.0.8.tar.gz` & `tmp/kgraph-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\kgraph-1.0.8.tar", last modified: Sat Oct 29 09:59:21 2022, max compression
+gzip compressed data, was "dist/kgraph-1.0.9.tar", last modified: Thu Jun  8 05:34:12 2023, max compression
```

## Comparing `kgraph-1.0.8.tar` & `kgraph-1.0.9.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxrwxrwx   0        0        0        0 2022-10-29 09:59:21.000000 kgraph-1.0.8/
--rw-rw-rw-   0        0        0    11341 2022-04-03 08:04:50.000000 kgraph-1.0.8/LICENSE
--rw-rw-rw-   0        0        0       78 2022-04-03 08:16:07.000000 kgraph-1.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      601 2022-10-29 09:59:21.000000 kgraph-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0        0 2022-07-06 10:06:46.000000 kgraph-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2022-10-29 09:59:21.000000 kgraph-1.0.8/kgraph/
--rw-rw-rw-   0        0        0    14602 2022-10-28 13:41:22.000000 kgraph-1.0.8/kgraph/__init__.py
--rw-rw-rw-   0        0        0      487 2022-05-25 14:48:14.000000 kgraph-1.0.8/kgraph/__init__.pyi
--rw-rw-rw-   0        0        0     5639 2022-10-28 15:16:58.000000 kgraph-1.0.8/kgraph/log.py
-drwxrwxrwx   0        0        0        0 2022-10-29 09:59:21.000000 kgraph-1.0.8/kgraph/loss/
--rw-rw-rw-   0        0        0      984 2022-05-26 13:41:20.000000 kgraph-1.0.8/kgraph/loss/Loss.py
--rw-rw-rw-   0        0        0     1668 2022-05-26 13:41:40.000000 kgraph-1.0.8/kgraph/loss/MarginLoss.py
--rw-rw-rw-   0        0        0     1785 2022-05-26 13:41:59.000000 kgraph-1.0.8/kgraph/loss/SigmoidLoss.py
--rw-rw-rw-   0        0        0     1674 2022-05-26 13:42:25.000000 kgraph-1.0.8/kgraph/loss/SoftplusLoss.py
--rw-rw-rw-   0        0        0      343 2022-05-26 13:40:51.000000 kgraph-1.0.8/kgraph/loss/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-29 09:59:21.000000 kgraph-1.0.8/kgraph/utils/
--rw-rw-rw-   0        0        0     5078 2022-09-08 15:38:15.000000 kgraph-1.0.8/kgraph/utils/__init__.py
--rw-rw-rw-   0        0        0   976614 2022-10-29 09:59:09.000000 kgraph-1.0.8/kgraph/utils/classification.cpp
--rw-rw-rw-   0        0        0     5500 2022-09-07 16:24:24.000000 kgraph-1.0.8/kgraph/utils/classification.pyx
--rw-rw-rw-   0        0        0   796070 2022-10-29 09:59:11.000000 kgraph-1.0.8/kgraph/utils/corrupt.cpp
--rw-rw-rw-   0        0        0      867 2022-06-04 06:14:40.000000 kgraph-1.0.8/kgraph/utils/corrupt.pxd
--rw-rw-rw-   0        0        0     4674 2022-06-04 06:14:59.000000 kgraph-1.0.8/kgraph/utils/corrupt.pyx
--rw-rw-rw-   0        0        0  1402887 2022-10-29 09:59:14.000000 kgraph-1.0.8/kgraph/utils/evaluation.cpp
--rw-rw-rw-   0        0        0    33756 2022-06-01 09:19:41.000000 kgraph-1.0.8/kgraph/utils/evaluation.pyx
--rw-rw-rw-   0        0        0  1013051 2022-10-29 09:59:16.000000 kgraph-1.0.8/kgraph/utils/memory.cpp
--rw-rw-rw-   0        0        0     4806 2022-06-07 09:56:40.000000 kgraph-1.0.8/kgraph/utils/memory.pxd
--rw-rw-rw-   0        0        0     9990 2022-06-07 09:56:50.000000 kgraph-1.0.8/kgraph/utils/memory.pyx
--rw-rw-rw-   0        0        0  1424467 2022-10-29 09:59:18.000000 kgraph-1.0.8/kgraph/utils/read.cpp
--rw-rw-rw-   0        0        0     2990 2022-09-07 16:21:07.000000 kgraph-1.0.8/kgraph/utils/read.pxd
--rw-rw-rw-   0        0        0    35316 2022-10-28 13:50:13.000000 kgraph-1.0.8/kgraph/utils/read.pyx
--rw-rw-rw-   0        0        0  1258902 2022-10-29 09:59:20.000000 kgraph-1.0.8/kgraph/utils/sample.cpp
--rw-rw-rw-   0        0        0    21956 2022-09-08 16:21:55.000000 kgraph-1.0.8/kgraph/utils/sample.pyx
--rw-rw-rw-   0        0        0      435 2022-05-25 14:48:45.000000 kgraph-1.0.8/kgraph/utils/setup.py
--rw-rw-rw-   0        0        0   692002 2022-10-29 09:59:21.000000 kgraph-1.0.8/kgraph/utils/tools.cpp
--rw-rw-rw-   0        0        0     9022 2022-09-07 13:54:13.000000 kgraph-1.0.8/kgraph/utils/tools.pyx
-drwxrwxrwx   0        0        0        0 2022-10-29 09:59:21.000000 kgraph-1.0.8/kgraph.egg-info/
--rw-rw-rw-   0        0        0      601 2022-10-29 09:59:21.000000 kgraph-1.0.8/kgraph.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1056 2022-10-29 09:59:21.000000 kgraph-1.0.8/kgraph.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-29 09:59:21.000000 kgraph-1.0.8/kgraph.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-05-26 02:51:07.000000 kgraph-1.0.8/kgraph.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       93 2022-10-29 09:59:21.000000 kgraph-1.0.8/kgraph.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-10-29 09:59:21.000000 kgraph-1.0.8/kgraph.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      942 2022-10-29 09:59:21.000000 kgraph-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     4691 2022-09-09 08:26:37.000000 kgraph-1.0.8/setup.py
+drwxrwxrwx   0 long      (1000) long      (1000)        0 2023-06-08 05:34:11.000000 kgraph-1.0.9/
+-rwxrwxrwx   0 long      (1000) long      (1000)    11341 2022-04-03 08:04:50.000000 kgraph-1.0.9/LICENSE
+-rwxrwxrwx   0 long      (1000) long      (1000)       78 2022-04-03 08:16:07.000000 kgraph-1.0.9/MANIFEST.in
+-rwxrwxrwx   0 long      (1000) long      (1000)     1847 2023-06-08 05:34:11.000000 kgraph-1.0.9/PKG-INFO
+-rwxrwxrwx   0 long      (1000) long      (1000)     1228 2022-10-30 10:58:16.000000 kgraph-1.0.9/README.md
+drwxrwxrwx   0 long      (1000) long      (1000)        0 2023-06-08 05:34:11.000000 kgraph-1.0.9/kgraph/
+-rwxrwxrwx   0 long      (1000) long      (1000)    16423 2023-06-08 03:22:38.000000 kgraph-1.0.9/kgraph/__init__.py
+-rwxrwxrwx   0 long      (1000) long      (1000)      487 2022-05-25 14:48:14.000000 kgraph-1.0.9/kgraph/__init__.pyi
+-rwxrwxrwx   0 long      (1000) long      (1000)     4696 2023-06-08 02:55:51.000000 kgraph-1.0.9/kgraph/log.py
+drwxrwxrwx   0 long      (1000) long      (1000)        0 2023-06-08 05:34:11.000000 kgraph-1.0.9/kgraph/loss/
+-rwxrwxrwx   0 long      (1000) long      (1000)      984 2022-05-26 13:41:20.000000 kgraph-1.0.9/kgraph/loss/Loss.py
+-rwxrwxrwx   0 long      (1000) long      (1000)     1668 2022-05-26 13:41:40.000000 kgraph-1.0.9/kgraph/loss/MarginLoss.py
+-rwxrwxrwx   0 long      (1000) long      (1000)     1785 2022-05-26 13:41:59.000000 kgraph-1.0.9/kgraph/loss/SigmoidLoss.py
+-rwxrwxrwx   0 long      (1000) long      (1000)     1674 2022-05-26 13:42:25.000000 kgraph-1.0.9/kgraph/loss/SoftplusLoss.py
+-rwxrwxrwx   0 long      (1000) long      (1000)      343 2022-05-26 13:40:51.000000 kgraph-1.0.9/kgraph/loss/__init__.py
+-rwxrwxrwx   0 long      (1000) long      (1000)     2322 2023-06-08 03:31:25.000000 kgraph-1.0.9/kgraph/nn.py
+drwxrwxrwx   0 long      (1000) long      (1000)        0 2023-06-08 05:34:11.000000 kgraph-1.0.9/kgraph/utils/
+-rwxrwxrwx   0 long      (1000) long      (1000)     5078 2022-09-08 15:38:15.000000 kgraph-1.0.9/kgraph/utils/__init__.py
+-rwxrwxrwx   0 long      (1000) long      (1000)   986641 2023-06-08 05:06:28.000000 kgraph-1.0.9/kgraph/utils/classification.cpp
+-rwxrwxrwx   0 long      (1000) long      (1000)     5500 2022-09-07 16:24:24.000000 kgraph-1.0.9/kgraph/utils/classification.pyx
+-rwxrwxrwx   0 long      (1000) long      (1000)   796069 2023-06-08 05:06:29.000000 kgraph-1.0.9/kgraph/utils/corrupt.cpp
+-rwxrwxrwx   0 long      (1000) long      (1000)      867 2022-06-04 06:14:40.000000 kgraph-1.0.9/kgraph/utils/corrupt.pxd
+-rwxrwxrwx   0 long      (1000) long      (1000)     4674 2022-06-04 06:14:59.000000 kgraph-1.0.9/kgraph/utils/corrupt.pyx
+-rwxrwxrwx   0 long      (1000) long      (1000)  1412914 2023-06-08 05:06:30.000000 kgraph-1.0.9/kgraph/utils/evaluation.cpp
+-rwxrwxrwx   0 long      (1000) long      (1000)    33756 2022-06-01 09:19:41.000000 kgraph-1.0.9/kgraph/utils/evaluation.pyx
+-rwxrwxrwx   0 long      (1000) long      (1000)  1013056 2023-06-08 05:06:32.000000 kgraph-1.0.9/kgraph/utils/memory.cpp
+-rwxrwxrwx   0 long      (1000) long      (1000)     4806 2022-06-07 09:56:40.000000 kgraph-1.0.9/kgraph/utils/memory.pxd
+-rwxrwxrwx   0 long      (1000) long      (1000)     9990 2022-06-07 09:56:50.000000 kgraph-1.0.9/kgraph/utils/memory.pyx
+-rwxrwxrwx   0 long      (1000) long      (1000)  1436868 2023-06-08 05:06:33.000000 kgraph-1.0.9/kgraph/utils/read.cpp
+-rwxrwxrwx   0 long      (1000) long      (1000)     2990 2022-09-07 16:21:07.000000 kgraph-1.0.9/kgraph/utils/read.pxd
+-rwxrwxrwx   0 long      (1000) long      (1000)    36214 2022-10-30 11:15:38.000000 kgraph-1.0.9/kgraph/utils/read.pyx
+-rwxrwxrwx   0 long      (1000) long      (1000)  1268931 2023-06-08 05:06:34.000000 kgraph-1.0.9/kgraph/utils/sample.cpp
+-rwxrwxrwx   0 long      (1000) long      (1000)    21956 2022-09-08 16:21:55.000000 kgraph-1.0.9/kgraph/utils/sample.pyx
+-rwxrwxrwx   0 long      (1000) long      (1000)      435 2022-05-25 14:48:45.000000 kgraph-1.0.9/kgraph/utils/setup.py
+-rwxrwxrwx   0 long      (1000) long      (1000)   702060 2023-06-08 05:06:35.000000 kgraph-1.0.9/kgraph/utils/tools.cpp
+-rwxrwxrwx   0 long      (1000) long      (1000)     9022 2022-09-07 13:54:13.000000 kgraph-1.0.9/kgraph/utils/tools.pyx
+drwxrwxrwx   0 long      (1000) long      (1000)        0 2023-06-08 05:34:11.000000 kgraph-1.0.9/kgraph.egg-info/
+-rwxrwxrwx   0 long      (1000) long      (1000)     1847 2023-06-08 05:34:09.000000 kgraph-1.0.9/kgraph.egg-info/PKG-INFO
+-rwxrwxrwx   0 long      (1000) long      (1000)      891 2023-06-08 05:34:09.000000 kgraph-1.0.9/kgraph.egg-info/SOURCES.txt
+-rwxrwxrwx   0 long      (1000) long      (1000)        1 2023-06-08 05:34:09.000000 kgraph-1.0.9/kgraph.egg-info/dependency_links.txt
+-rwxrwxrwx   0 long      (1000) long      (1000)        2 2022-05-26 02:51:07.000000 kgraph-1.0.9/kgraph.egg-info/not-zip-safe
+-rwxrwxrwx   0 long      (1000) long      (1000)       93 2023-06-08 05:34:09.000000 kgraph-1.0.9/kgraph.egg-info/requires.txt
+-rwxrwxrwx   0 long      (1000) long      (1000)        7 2023-06-08 05:34:09.000000 kgraph-1.0.9/kgraph.egg-info/top_level.txt
+-rwxrwxrwx   0 long      (1000) long      (1000)      900 2023-06-08 05:34:11.000000 kgraph-1.0.9/setup.cfg
+-rwxrwxrwx   0 long      (1000) long      (1000)     4834 2023-06-08 05:06:19.000000 kgraph-1.0.9/setup.py
```

### Comparing `kgraph-1.0.8/LICENSE` & `kgraph-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kgraph-1.0.8/kgraph/__init__.py` & `kgraph-1.0.9/kgraph/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,67 +19,64 @@
 
 class Data(DataSet):
     
     def __init__(self, num_ent: int=0, num_rel: int=0):
         super(Data, self).__init__(num_ent, num_rel)
         self.no_sort = True
     
-    def load(self, path: str, no_sort: bool=True) -> None:
+    def load(self, path: str, no_sort: bool = True) -> None:
+        """
+        Load the dataset from the provided path.
+
+        Args:
+            path (str): The path to the dataset.
+            no_sort (bool, optional): If True, the dataset will not be sorted. Defaults to True.
+
+        Returns:
+            None
+        """
         path += '/'
-        
-        if isinstance(path, str):
-            path = path.encode('utf-8')
-        if isinstance(path, bytes):
-            super(Data, self).load(path, int(no_sort))
-            # self.__calculate_train_data_size()
-        else:
+        path = path.encode('utf-8') if isinstance(path, str) else path
+        try:
+            super().load(path, int(no_sort))
+            self.path = path.decode('utf-8')
+            self.no_sort = no_sort
+        except FileNotFoundError:
             print('Can not find the dataset.')
-        self.path = path.decode('utf-8')
-        
-        self.no_sort = no_sort
-        # print('ok')
     
     def load_description(self):
+        """
+        Loads the entity and relation descriptions from files in the given path.
+        If `no_sort` is True, it loads the unsorted versions of the files.
+        Returns two dictionaries: `ent_id2text` maps entity IDs to their descriptions,
+        and `rel_id2text` maps relation IDs to their descriptions.
+        """
         entity2id_file_name = 'entity2id_no_sort.txt' if self.no_sort else 'entity2id_on_sort.txt'
         relation2id_file_name = 'relation2id_no_sort.txt' if self.no_sort else 'relation2id_on_sort.txt'
-        
         entity2id_file_name = os.path.join(self.path, entity2id_file_name)
         relation2id_file_name = os.path.join(self.path, relation2id_file_name)
-        
-        ent2id = {}
-        with open(entity2id_file_name, 'r', encoding='utf-8') as f:
-            f.readline()
-            for line in f.readlines():
-                line = line.strip().split('\t')
-                # print(line)
-                ent2id[line[0]] = int(line[1])
-        
-        rel2id = {}
-        with open(relation2id_file_name, 'r', encoding='utf-8') as f:
-            f.readline()
-            for line in f.readlines():
-                line = line.strip().split('\t')
-                rel2id[line[0]] = int(line[1])
-        
-        ent2text = os.path.join(self.path, 'ent2text.txt')
-        rel2text = os.path.join(self.path, 'rel2text.txt')
-        
-        ent_id2text = {}
-        rel_id2text = {}
-        with open(ent2text, 'r', encoding='utf-8') as f:
-            for line in f.readlines():
-                line = line.strip().split('\t')
-                if ent2id.get(line[0], None) is not None:
-                    ent_id2text[ent2id[line[0]]] = line[1]
-        with open(rel2text, 'r', encoding='utf-8') as f:
-            for line in f.readlines():
-                line = line.strip().split('\t')
-                if rel2id.get(line[0], None) is not None:
-                    rel_id2text[rel2id[line[0]]] = line[1]
-        
+
+        ent2id = {line[0]: int(line[1]) for line in [line.strip().split('\t') for line in open(
+            entity2id_file_name, 'r', encoding='utf-8').readlines()[1:]]}
+        rel2id = {line[0]: int(line[1]) for line in [line.strip().split('\t') for line in open(
+            relation2id_file_name, 'r', encoding='utf-8').readlines()[1:]]}
+
+        ent_id2text = {ent2id[line[0]]: line[1] for line in [line.strip().split('\t') for line in open(
+            os.path.join(self.path, 'ent2text.txt'), 'r', encoding='utf-8').readlines()] if line[0] in ent2id}
+        rel_id2text = {rel2id[line[0]]: line[1] for line in [line.strip().split('\t') for line in open(
+            os.path.join(self.path, 'rel2text.txt'), 'r', encoding='utf-8').readlines()] if line[0] in rel2id}
+
+        if os.path.exists(os.path.join(self.path, 'ent2name.txt')):
+            ent2name = {line[0]: line[1] for line in [line.strip().split('\t') for line in open(
+                os.path.join(self.path, 'ent2name.txt'), 'r', encoding='utf-8').readlines()] if line[0] in ent2id}
+            
+            for k, v in ent2id.items():
+                if v not in ent_id2text:
+                    ent_id2text[v] = ent2name[k]
+
         return ent_id2text, rel_id2text
     
     def generateN2N(self) -> None:
         if not os.path.exists(os.path.join(self.path, 'constraint.txt')):
             generateN2N(self.train, self.valid, self.test, self.path)
     
     def clean(self):
@@ -115,44 +112,80 @@
     @property
     def multi2multi(self):
         return self.__load_triple_from_file__('n-n.txt')
         
         
 class FB15k(Data):
     def __init__(self, path: str=None, no_sort: bool=True) -> None:
+        """
+        Initializes the FB15k dataset with optional path and sorting parameters.
+
+        Args:
+            path (str): The path to the dataset directory. Defaults to 'data/'.
+            no_sort (bool): Whether to sort the dataset. Defaults to True.
+
+        Returns:
+            None
+        """
         path = 'data/' if path is None else path
         url='https://raw.githubusercontent.com/pp413/Knowledge_embedding_benchmark_datasets/main/FB15k.zip'
         super(FB15k, self).__init__()
         super(FB15k, self).load(*load_data(url, path, no_sort=no_sort))
         super(FB15k, self).resetPosAndNegValid(False)
         super(FB15k, self).resetPosAndNegTest(False)
         super(FB15k, self).generateN2N()
 
 class FB15k237(Data):
     def __init__(self, path: str=None, no_sort: bool=True) -> None:
+        """
+        Initializes an instance of the FB15k237 class.
+
+        Args:
+            path (str, optional): The path to the data directory. Defaults to 'data/'.
+            no_sort (bool, optional): If True, the loaded data is not sorted. Defaults to True.
+
+        Returns:
+            None
+        """
         path = 'data/' if path is None else path
         url='https://raw.githubusercontent.com/pp413/Knowledge_embedding_benchmark_datasets/main/FB15k-237.zip'
         super(FB15k237, self).__init__()
         super(FB15k237, self).load(*load_data(url, path, no_sort=no_sort))
         super(FB15k237, self).resetPosAndNegValid(False)
         super(FB15k237, self).resetPosAndNegTest(False)
         super(FB15k237, self).generateN2N()
 
 class WN18(Data):
     def __init__(self, path: str=None, no_sort: bool=True) -> None:
+        """
+        Initializes the WN18 dataset object which inherits from the base dataset class.
+        :param path: A string representing the path to the dataset files. If `None`, defaults to 'data/'.
+        :param no_sort: A boolean indicating whether to sort the data or not. Defaults to `True`.
+        :return: None
+        """
         path = 'data/' if path is None else path
         url='https://raw.githubusercontent.com/pp413/Knowledge_embedding_benchmark_datasets/main/WN18.zip'
         super(WN18, self).__init__()
         super(WN18, self).load(*load_data(url, path, no_sort=no_sort))
         super(WN18, self).resetPosAndNegValid(False)
         super(WN18, self).resetPosAndNegTest(False)
         super(WN18, self).generateN2N()
 
 class WN18RR(Data):
     def __init__(self, path: str=None, no_sort: bool=True) -> None:
+        """
+        Initializes a new instance of the WN18RR class.
+
+        :param path: The path to the data directory. If None, defaults to 'data/'.
+        :type path: str
+        :param no_sort: Whether to sort the data.
+        :type no_sort: bool
+        :return: None
+        :rtype: None
+        """
         path = 'data/' if path is None else path
         url='https://raw.githubusercontent.com/pp413/Knowledge_embedding_benchmark_datasets/main/WN18RR.zip'
         super(WN18RR, self).__init__()
         super(WN18RR, self).load(*load_data(url, path, no_sort=no_sort))
         super(WN18RR, self).resetPosAndNegValid(False)
         super(WN18RR, self).resetPosAndNegTest(False)
         super(WN18RR, self).generateN2N()
@@ -287,14 +320,16 @@
         return:
             the table of results of N2N.
         '''
         
         results = {'1to1': [], '1toN': [], 'Nto1': [], 'NtoN': []}
         data = self.data
         
+        test = self.data.test
+        
         # 1 to 1
         self.data.test = data.one2one
         # print('1 to 1')
         results['1to1'] += [i for i in self.__predict_test(function, self.data, batch_size)]
         
         # 1 to n
         self.data.test = data.one2multi
@@ -307,14 +342,16 @@
         results['Nto1'] += [i for i in self.__predict_test(function, self.data, batch_size)]
         
         # n to n
         self.data.test = data.multi2multi
         # print('n to n')
         results['NtoN'] += [i for i in self.__predict_test(function, self.data, batch_size)]
         
+        self.data.test = test
+        
         return log_N2N(results, data_name=self.data_name)
 
     def calculate_classification_accuracy(self, function, batch_size=1000, threshold=None):
         '''
         Calculate the classification accuracy.
         Params:
             function: the prediction function.
```

### Comparing `kgraph-1.0.8/kgraph/log.py` & `kgraph-1.0.9/kgraph/log.py`

 * *Files 22% similar despite different names*

```diff
@@ -49,46 +49,14 @@
     std_out_format = '%(asctime)s - [%(levelname)s] - %(message)s'
     consoleHandler = logging.StreamHandler(sys.stdout)
     consoleHandler.setFormatter(logging.Formatter(std_out_format))
     logger.addHandler(consoleHandler)
     
     return logger
 
-# class Logger(Live):
-#     '''
-#     From dvclive.Live
-#     Logger.log()
-#     Logger.log_image()
-#     Logger.log_plot()
-#     Logger.make_report()
-#     Logger.get_step()
-#     Logger.next_step()
-#     Logger.set_step()
-    
-#     '''
-    
-#     def __init__(self, log_name: Optional[str] = "Model",
-#                  path: Optional[str] = "log",
-#                  resume: bool = False,
-#                  report: Optional[str] = "auto"):
-#         '''
-#         log_name: the name of the log file;
-#         path: the dir path;
-#         resume: True or False;
-#         report: .
-#         '''
-#         super(Logger, self).__init__(path=path, resume=resume, report=report)
-#         self.logger = set_logger(log_name, log_dir=path)
-    
-#     def info(self, message: Optional[str]):
-#         self.logger.info(message)
-    
-#     def log(path_name, p):
-#         super(Logger, self).log(path_name, p)
-
 #
 def get_result_table(rhs_ranks, rhs_franks, lhs_ranks, lhs_franks, data_name='benchmark', flags='Valid'):
     """
     rhs: predict the tails of triples
     lhs: predict the heads of triples
     """
```

### Comparing `kgraph-1.0.8/kgraph/loss/Loss.py` & `kgraph-1.0.9/kgraph/loss/Loss.py`

 * *Files identical despite different names*

### Comparing `kgraph-1.0.8/kgraph/loss/MarginLoss.py` & `kgraph-1.0.9/kgraph/loss/MarginLoss.py`

 * *Files identical despite different names*

### Comparing `kgraph-1.0.8/kgraph/loss/SigmoidLoss.py` & `kgraph-1.0.9/kgraph/loss/SigmoidLoss.py`

 * *Files identical despite different names*

### Comparing `kgraph-1.0.8/kgraph/loss/SoftplusLoss.py` & `kgraph-1.0.9/kgraph/loss/SoftplusLoss.py`

 * *Files identical despite different names*

### Comparing `kgraph-1.0.8/kgraph/utils/__init__.py` & `kgraph-1.0.9/kgraph/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kgraph-1.0.8/kgraph/utils/classification.cpp` & `kgraph-1.0.9/kgraph/utils/classification.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 /* Generated by Cython 0.29.28 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "C:\\ProgramData\\Miniconda3\\include\\Python.h",
-            "C:\\ProgramData\\Miniconda3\\lib\\site-packages\\numpy\\core\\include\\numpy\\arrayobject.h",
-            "C:\\ProgramData\\Miniconda3\\lib\\site-packages\\numpy\\core\\include\\numpy\\ufuncobject.h"
+            "/home/long/miniconda3/include/python3.7m/Python.h",
+            "/home/long/miniconda3/lib/python3.7/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/home/long/miniconda3/lib/python3.7/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/home/long/miniconda3/lib/python3.7/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/home/long/miniconda3/lib/python3.7/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/home/long/miniconda3/lib/python3.7/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "extra_compile_args": [
             "-std=c++11"
         ],
         "include_dirs": [
-            "C:\\ProgramData\\Miniconda3\\lib\\site-packages\\numpy\\core\\include",
-            "C:\\ProgramData\\Miniconda3\\include"
+            "/home/long/miniconda3/lib/python3.7/site-packages/numpy/core/include",
+            "/home/long/miniconda3/include/python3.7m"
         ],
         "language": "c++",
         "name": "kgraph.utils.classification",
         "sources": [
             "kgraph/utils/classification.pyx"
         ]
     },
@@ -720,14 +723,17 @@
 
 #define __PYX_HAVE__kgraph__utils__classification
 #define __PYX_HAVE_API__kgraph__utils__classification
 /* Early includes */
 #include <string.h>
 #include <stdio.h>
 #include "numpy/arrayobject.h"
+#include "numpy/ndarrayobject.h"
+#include "numpy/ndarraytypes.h"
+#include "numpy/arrayscalars.h"
 #include "numpy/ufuncobject.h"
 
     /* NumPy API declarations from "numpy/__init__.pxd" */
     
 #include <stdlib.h>
 #include "ios"
 #include "new"
@@ -965,20 +971,20 @@
 #if CYTHON_CCOMPLEX && !defined(__cplusplus) && defined(__sun__) && defined(__GNUC__)
   #undef _Complex_I
   #define _Complex_I 1.0fj
 #endif
 
 
 static const char *__pyx_f[] = {
-  "kgraph\\utils\\classification.pyx",
+  "kgraph/utils/classification.pyx",
   "__init__.pxd",
   "stringsource",
   "type.pxd",
-  "kgraph\\utils\\memory.pxd",
-  "kgraph\\utils\\read.pxd",
+  "kgraph/utils/memory.pxd",
+  "kgraph/utils/read.pxd",
 };
 /* MemviewSliceStruct.proto */
 struct __pyx_memoryview_obj;
 typedef struct {
   struct __pyx_memoryview_obj *memview;
   char *data;
   Py_ssize_t shape[8];
@@ -1081,195 +1087,195 @@
 #define __Pyx_PyGILState_Ensure PyGILState_Ensure
 #define __Pyx_PyGILState_Release PyGILState_Release
 #define __Pyx_FastGIL_Remember()
 #define __Pyx_FastGIL_Forget()
 #define __Pyx_FastGilFuncInit()
 
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":689
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":690
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":690
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":691
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":691
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":692
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":693
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":696
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":697
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":697
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":698
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":698
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":699
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":700
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":703
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":704
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":704
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":705
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":713
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":714
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":714
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":715
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":715
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":716
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":717
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":718
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":719
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":720
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":721
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":722
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":722
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":723
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":724
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":725
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":726
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1306,42 +1312,42 @@
 struct __pyx_obj_6kgraph_5utils_6memory_MemoryPool;
 struct __pyx_obj_6kgraph_5utils_4read_DataSet;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":728
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":729
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":730
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":730
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":732
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":733
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2712,14 +2718,24 @@
 /* Module declarations from 'numpy' */
 
 /* Module declarations from 'numpy' */
 static PyTypeObject *__pyx_ptype_5numpy_dtype = 0;
 static PyTypeObject *__pyx_ptype_5numpy_flatiter = 0;
 static PyTypeObject *__pyx_ptype_5numpy_broadcast = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ndarray = 0;
+static PyTypeObject *__pyx_ptype_5numpy_generic = 0;
+static PyTypeObject *__pyx_ptype_5numpy_number = 0;
+static PyTypeObject *__pyx_ptype_5numpy_integer = 0;
+static PyTypeObject *__pyx_ptype_5numpy_signedinteger = 0;
+static PyTypeObject *__pyx_ptype_5numpy_unsignedinteger = 0;
+static PyTypeObject *__pyx_ptype_5numpy_inexact = 0;
+static PyTypeObject *__pyx_ptype_5numpy_floating = 0;
+static PyTypeObject *__pyx_ptype_5numpy_complexfloating = 0;
+static PyTypeObject *__pyx_ptype_5numpy_flexible = 0;
+static PyTypeObject *__pyx_ptype_5numpy_character = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ufunc = 0;
 
 /* Module declarations from 'libc.stdlib' */
 
 /* Module declarations from 'libcpp.vector' */
 
 /* Module declarations from 'kgraph.utils.memory' */
@@ -2946,15 +2962,15 @@
 static const char __pyx_k_Cannot_index_with_type_s[] = "Cannot index with type '%s'";
 static const char __pyx_k_Invalid_shape_in_axis_d_d[] = "Invalid shape in axis %d: %d.";
 static const char __pyx_k_run_triple_classification[] = "run_triple_classification";
 static const char __pyx_k_itemsize_0_for_cython_array[] = "itemsize <= 0 for cython.array";
 static const char __pyx_k_kgraph_utils_classification[] = "kgraph.utils.classification";
 static const char __pyx_k_unable_to_allocate_array_data[] = "unable to allocate array data.";
 static const char __pyx_k_strided_and_direct_or_indirect[] = "<strided and direct or indirect>";
-static const char __pyx_k_kgraph_utils_classification_pyx[] = "kgraph\\utils\\classification.pyx";
+static const char __pyx_k_kgraph_utils_classification_pyx[] = "kgraph/utils/classification.pyx";
 static const char __pyx_k_numpy_core_multiarray_failed_to[] = "numpy.core.multiarray failed to import";
 static const char __pyx_k_Buffer_view_does_not_expose_stri[] = "Buffer view does not expose strides";
 static const char __pyx_k_Can_only_create_a_buffer_that_is[] = "Can only create a buffer that is contiguous in memory.";
 static const char __pyx_k_Cannot_assign_to_read_only_memor[] = "Cannot assign to read-only memoryview";
 static const char __pyx_k_Cannot_create_writable_memory_vi[] = "Cannot create writable memory view from read-only memoryview";
 static const char __pyx_k_Empty_shape_tuple_for_cython_arr[] = "Empty shape tuple for cython.array";
 static const char __pyx_k_Incompatible_checksums_s_vs_0xb0[] = "Incompatible checksums (%s vs 0xb068931 = (name))";
@@ -5316,15 +5332,15 @@
   __Pyx_WriteUnraisable("kgraph.utils.classification.get_best_threshold", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __Pyx_pretend_to_initialize(&__pyx_r);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":734
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -5333,29 +5349,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":735
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":736
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 736, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":734
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -5366,15 +5382,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":737
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -5383,29 +5399,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":738
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":739
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 739, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":737
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -5416,15 +5432,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":740
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -5433,29 +5449,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":741
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":742
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 742, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":740
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -5466,15 +5482,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":743
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -5483,29 +5499,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":744
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":745
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 745, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":743
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -5516,15 +5532,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":746
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -5533,29 +5549,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":747
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":748
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 748, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":746
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -5566,212 +5582,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":749
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":750
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":751
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":752
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":750
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":753
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":754
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":749
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":868
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":869
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":870
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":931
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":868
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":872
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":873
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":934
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":874
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":875
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":936
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":874
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":876
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":937
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":872
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":880
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -5787,15 +5803,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":881
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -5803,84 +5819,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":882
+      /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":943
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 882, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 943, __pyx_L3_error)
 
-      /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":881
+      /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":883
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":944
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 883, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":884
+      /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 884, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 945, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 884, __pyx_L5_except_error)
+      __PYX_ERR(1, 945, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":881
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":880
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -5895,15 +5911,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":886
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5919,15 +5935,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":887
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5935,84 +5951,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":888
+      /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":949
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 888, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 949, __pyx_L3_error)
 
-      /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":887
+      /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":889
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":950
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 889, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":890
+      /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 890, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 951, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 890, __pyx_L5_except_error)
+      __PYX_ERR(1, 951, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":887
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":886
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6027,15 +6043,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":892
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6051,15 +6067,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":893
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -6067,84 +6083,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":894
+      /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":955
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 894, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 955, __pyx_L3_error)
 
-      /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":893
+      /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":895
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":956
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 895, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":896
+      /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":957
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 896, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 957, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 896, __pyx_L5_except_error)
+      __PYX_ERR(1, 957, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":893
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":892
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6159,14 +6175,188 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":967
+ * 
+ * 
+ * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.timedelta64)`
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":979
+ *     bool
+ *     """
+ *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
+  goto __pyx_L0;
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":967
+ * 
+ * 
+ * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.timedelta64)`
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":982
+ * 
+ * 
+ * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.datetime64)`
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("is_datetime64_object", 0);
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":994
+ *     bool
+ *     """
+ *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
+  goto __pyx_L0;
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":982
+ * 
+ * 
+ * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.datetime64)`
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":997
+ * 
+ * 
+ * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy datetime64 object
+ */
+
+static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
+  npy_datetime __pyx_r;
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":1004
+ *     also needed.  That can be found using `get_datetime64_unit`.
+ *     """
+ *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
+  goto __pyx_L0;
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":997
+ * 
+ * 
+ * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy datetime64 object
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":1007
+ * 
+ * 
+ * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ */
+
+static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
+  npy_timedelta __pyx_r;
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":1011
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ *     """
+ *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
+  goto __pyx_L0;
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":1007
+ * 
+ * 
+ * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":1014
+ * 
+ * 
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ */
+
+static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
+  NPY_DATETIMEUNIT __pyx_r;
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":1018
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ *     """
+ *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
+ */
+  __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
+  goto __pyx_L0;
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":1014
+ * 
+ * 
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
 /* "View.MemoryView":122
  *         cdef bint dtype_is_object
  * 
  *     def __cinit__(array self, tuple shape, Py_ssize_t itemsize, format not None,             # <<<<<<<<<<<<<<
  *                   mode="c", bint allocate_buffer=True):
  * 
  */
@@ -20448,15 +20638,15 @@
   {&__pyx_kp_s_unable_to_allocate_shape_and_str, __pyx_k_unable_to_allocate_shape_and_str, sizeof(__pyx_k_unable_to_allocate_shape_and_str), 0, 0, 1, 0},
   {&__pyx_n_s_unpack, __pyx_k_unpack, sizeof(__pyx_k_unpack), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 28, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 884, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 945, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(2, 133, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(2, 148, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(2, 151, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(2, 2, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(2, 404, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(2, 613, __pyx_L1_error)
   __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(2, 832, __pyx_L1_error)
@@ -20476,33 +20666,33 @@
  *         pbar.set_description("Classification:")
  * 
  */
   __pyx_tuple_ = PyTuple_Pack(3, Py_None, Py_None, Py_None); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":884
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 884, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 945, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":890
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 890, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 951, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
   /* "View.MemoryView":133
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
@@ -20907,26 +21097,46 @@
   sizeof(PyTypeObject),
   #else
   sizeof(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 200, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 200, __pyx_L1_error)
   __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 223, __pyx_L1_error)
   __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 227, __pyx_L1_error)
   __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 239, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 771, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 773, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 775, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 777, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 779, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 781, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 783, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 785, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 787, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 789, __pyx_L1_error)
   __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 764, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 827, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("kgraph.utils.memory"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_6kgraph_5utils_6memory_Memory = __Pyx_ImportType(__pyx_t_1, "kgraph.utils.memory", "Memory", sizeof(struct __pyx_obj_6kgraph_5utils_6memory_Memory), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_6kgraph_5utils_6memory_Memory) __PYX_ERR(4, 70, __pyx_L1_error)
   __pyx_ptype_6kgraph_5utils_6memory_Data = __Pyx_ImportType(__pyx_t_1, "kgraph.utils.memory", "Data", sizeof(struct __pyx_obj_6kgraph_5utils_6memory_Data), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_6kgraph_5utils_6memory_Data) __PYX_ERR(4, 75, __pyx_L1_error)
```

### Comparing `kgraph-1.0.8/kgraph/utils/classification.pyx` & `kgraph-1.0.9/kgraph/utils/classification.pyx`

 * *Files identical despite different names*

### Comparing `kgraph-1.0.8/kgraph/utils/corrupt.cpp` & `kgraph-1.0.9/kgraph/utils/corrupt.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 {
     "distutils": {
         "depends": [],
         "extra_compile_args": [
             "-std=c++11"
         ],
         "include_dirs": [
-            "C:\\ProgramData\\Miniconda3\\lib\\site-packages\\numpy\\core\\include",
-            "C:\\ProgramData\\Miniconda3\\include"
+            "/home/long/miniconda3/lib/python3.7/site-packages/numpy/core/include",
+            "/home/long/miniconda3/include/python3.7m"
         ],
         "language": "c++",
         "name": "kgraph.utils.corrupt",
         "sources": [
             "kgraph/utils/corrupt.pyx"
         ]
     },
@@ -934,16 +934,16 @@
 static int __pyx_clineno = 0;
 static const char * __pyx_cfilenm= __FILE__;
 static const char *__pyx_filename;
 
 
 static const char *__pyx_f[] = {
   "stringsource",
-  "kgraph\\utils\\corrupt.pyx",
-  "kgraph\\utils\\memory.pxd",
+  "kgraph/utils/corrupt.pyx",
+  "kgraph/utils/memory.pxd",
 };
 /* ForceInitThreads.proto */
 #ifndef __PYX_FORCE_INIT_THREADS
   #define __PYX_FORCE_INIT_THREADS 0
 #endif
 
 /* NoFastGil.proto */
```

### Comparing `kgraph-1.0.8/kgraph/utils/corrupt.pxd` & `kgraph-1.0.9/kgraph/utils/corrupt.pxd`

 * *Files identical despite different names*

### Comparing `kgraph-1.0.8/kgraph/utils/corrupt.pyx` & `kgraph-1.0.9/kgraph/utils/corrupt.pyx`

 * *Files identical despite different names*

### Comparing `kgraph-1.0.8/kgraph/utils/evaluation.cpp` & `kgraph-1.0.9/kgraph/utils/evaluation.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 /* Generated by Cython 0.29.28 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "C:\\ProgramData\\Miniconda3\\include\\Python.h",
-            "C:\\ProgramData\\Miniconda3\\lib\\site-packages\\numpy\\core\\include\\numpy\\arrayobject.h",
-            "C:\\ProgramData\\Miniconda3\\lib\\site-packages\\numpy\\core\\include\\numpy\\ufuncobject.h"
+            "/home/long/miniconda3/include/python3.7m/Python.h",
+            "/home/long/miniconda3/lib/python3.7/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/home/long/miniconda3/lib/python3.7/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/home/long/miniconda3/lib/python3.7/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/home/long/miniconda3/lib/python3.7/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/home/long/miniconda3/lib/python3.7/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "extra_compile_args": [
             "-std=c++11"
         ],
         "include_dirs": [
-            "C:\\ProgramData\\Miniconda3\\lib\\site-packages\\numpy\\core\\include",
-            "C:\\ProgramData\\Miniconda3\\include"
+            "/home/long/miniconda3/lib/python3.7/site-packages/numpy/core/include",
+            "/home/long/miniconda3/include/python3.7m"
         ],
         "language": "c++",
         "name": "kgraph.utils.evaluation",
         "sources": [
             "kgraph/utils/evaluation.pyx"
         ]
     },
@@ -720,14 +723,17 @@
 
 #define __PYX_HAVE__kgraph__utils__evaluation
 #define __PYX_HAVE_API__kgraph__utils__evaluation
 /* Early includes */
 #include <string.h>
 #include <stdio.h>
 #include "numpy/arrayobject.h"
+#include "numpy/ndarrayobject.h"
+#include "numpy/ndarraytypes.h"
+#include "numpy/arrayscalars.h"
 #include "numpy/ufuncobject.h"
 
     /* NumPy API declarations from "numpy/__init__.pxd" */
     
 #include <stdlib.h>
 #include "ios"
 #include "new"
@@ -965,20 +971,20 @@
 #if CYTHON_CCOMPLEX && !defined(__cplusplus) && defined(__sun__) && defined(__GNUC__)
   #undef _Complex_I
   #define _Complex_I 1.0fj
 #endif
 
 
 static const char *__pyx_f[] = {
-  "kgraph\\utils\\evaluation.pyx",
+  "kgraph/utils/evaluation.pyx",
   "__init__.pxd",
   "stringsource",
   "type.pxd",
-  "kgraph\\utils\\memory.pxd",
-  "kgraph\\utils\\read.pxd",
+  "kgraph/utils/memory.pxd",
+  "kgraph/utils/read.pxd",
 };
 /* MemviewSliceStruct.proto */
 struct __pyx_memoryview_obj;
 typedef struct {
   struct __pyx_memoryview_obj *memview;
   char *data;
   Py_ssize_t shape[8];
@@ -1081,195 +1087,195 @@
 #define __Pyx_PyGILState_Ensure PyGILState_Ensure
 #define __Pyx_PyGILState_Release PyGILState_Release
 #define __Pyx_FastGIL_Remember()
 #define __Pyx_FastGIL_Forget()
 #define __Pyx_FastGilFuncInit()
 
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":689
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":690
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":690
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":691
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":691
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":692
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":693
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":696
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":697
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":697
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":698
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":698
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":699
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":700
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":703
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":704
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":704
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":705
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":713
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":714
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":714
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":715
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":715
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":716
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":717
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":718
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":719
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":720
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":721
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":722
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":722
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":723
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":724
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":725
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":726
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1306,42 +1312,42 @@
 struct __pyx_obj_6kgraph_5utils_6memory_MemoryPool;
 struct __pyx_obj_6kgraph_5utils_4read_DataSet;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":728
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":729
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":730
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":730
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":732
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":733
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2710,14 +2716,24 @@
 /* Module declarations from 'numpy' */
 
 /* Module declarations from 'numpy' */
 static PyTypeObject *__pyx_ptype_5numpy_dtype = 0;
 static PyTypeObject *__pyx_ptype_5numpy_flatiter = 0;
 static PyTypeObject *__pyx_ptype_5numpy_broadcast = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ndarray = 0;
+static PyTypeObject *__pyx_ptype_5numpy_generic = 0;
+static PyTypeObject *__pyx_ptype_5numpy_number = 0;
+static PyTypeObject *__pyx_ptype_5numpy_integer = 0;
+static PyTypeObject *__pyx_ptype_5numpy_signedinteger = 0;
+static PyTypeObject *__pyx_ptype_5numpy_unsignedinteger = 0;
+static PyTypeObject *__pyx_ptype_5numpy_inexact = 0;
+static PyTypeObject *__pyx_ptype_5numpy_floating = 0;
+static PyTypeObject *__pyx_ptype_5numpy_complexfloating = 0;
+static PyTypeObject *__pyx_ptype_5numpy_flexible = 0;
+static PyTypeObject *__pyx_ptype_5numpy_character = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ufunc = 0;
 static CYTHON_INLINE int __pyx_f_5numpy_import_array(void); /*proto*/
 
 /* Module declarations from 'libc.stdlib' */
 
 /* Module declarations from 'libcpp.vector' */
 
@@ -2964,15 +2980,15 @@
 static const char __pyx_k_MemoryView_of_r_object[] = "<MemoryView of %r object>";
 static const char __pyx_k_MemoryView_of_r_at_0x_x[] = "<MemoryView of %r at 0x%x>";
 static const char __pyx_k_contiguous_and_indirect[] = "<contiguous and indirect>";
 static const char __pyx_k_kgraph_utils_evaluation[] = "kgraph.utils.evaluation";
 static const char __pyx_k_Cannot_index_with_type_s[] = "Cannot index with type '%s'";
 static const char __pyx_k_Invalid_shape_in_axis_d_d[] = "Invalid shape in axis %d: %d.";
 static const char __pyx_k_itemsize_0_for_cython_array[] = "itemsize <= 0 for cython.array";
-static const char __pyx_k_kgraph_utils_evaluation_pyx[] = "kgraph\\utils\\evaluation.pyx";
+static const char __pyx_k_kgraph_utils_evaluation_pyx[] = "kgraph/utils/evaluation.pyx";
 static const char __pyx_k_unable_to_allocate_array_data[] = "unable to allocate array data.";
 static const char __pyx_k_strided_and_direct_or_indirect[] = "<strided and direct or indirect>";
 static const char __pyx_k_numpy_core_multiarray_failed_to[] = "numpy.core.multiarray failed to import";
 static const char __pyx_k_Buffer_view_does_not_expose_stri[] = "Buffer view does not expose strides";
 static const char __pyx_k_Can_only_create_a_buffer_that_is[] = "Can only create a buffer that is contiguous in memory.";
 static const char __pyx_k_Cannot_assign_to_read_only_memor[] = "Cannot assign to read-only memoryview";
 static const char __pyx_k_Cannot_create_writable_memory_vi[] = "Cannot create writable memory view from read-only memoryview";
@@ -12943,15 +12959,15 @@
   __Pyx_XDECREF(__pyx_v_t_kwargs);
   __Pyx_XDECREF(__pyx_v_tbar);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":734
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -12960,29 +12976,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":735
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":736
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 736, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":734
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -12993,15 +13009,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":737
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -13010,29 +13026,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":738
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":739
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 739, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":737
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -13043,15 +13059,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":740
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -13060,29 +13076,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":741
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":742
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 742, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":740
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -13093,15 +13109,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":743
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -13110,29 +13126,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":744
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":745
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 745, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":743
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -13143,15 +13159,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":746
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -13160,29 +13176,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":747
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":748
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 748, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":746
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -13193,212 +13209,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":749
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":750
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":751
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":752
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":750
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":753
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":754
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":749
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":868
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":869
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":870
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":931
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":868
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":872
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":873
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":934
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":874
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":875
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":936
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":874
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":876
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":937
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":872
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":880
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -13414,15 +13430,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":881
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -13430,84 +13446,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":882
+      /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":943
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 882, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 943, __pyx_L3_error)
 
-      /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":881
+      /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":883
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":944
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 883, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":884
+      /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 884, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 945, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 884, __pyx_L5_except_error)
+      __PYX_ERR(1, 945, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":881
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":880
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -13522,15 +13538,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":886
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -13546,15 +13562,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":887
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -13562,84 +13578,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":888
+      /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":949
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 888, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 949, __pyx_L3_error)
 
-      /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":887
+      /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":889
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":950
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 889, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":890
+      /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 890, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 951, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 890, __pyx_L5_except_error)
+      __PYX_ERR(1, 951, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":887
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":886
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -13654,15 +13670,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":892
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -13678,15 +13694,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":893
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -13694,84 +13710,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":894
+      /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":955
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 894, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 955, __pyx_L3_error)
 
-      /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":893
+      /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":895
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":956
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 895, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":896
+      /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":957
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 896, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 957, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 896, __pyx_L5_except_error)
+      __PYX_ERR(1, 957, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":893
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":892
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -13786,14 +13802,188 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":967
+ * 
+ * 
+ * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.timedelta64)`
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":979
+ *     bool
+ *     """
+ *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
+  goto __pyx_L0;
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":967
+ * 
+ * 
+ * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.timedelta64)`
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":982
+ * 
+ * 
+ * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.datetime64)`
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("is_datetime64_object", 0);
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":994
+ *     bool
+ *     """
+ *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
+  goto __pyx_L0;
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":982
+ * 
+ * 
+ * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.datetime64)`
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":997
+ * 
+ * 
+ * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy datetime64 object
+ */
+
+static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
+  npy_datetime __pyx_r;
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":1004
+ *     also needed.  That can be found using `get_datetime64_unit`.
+ *     """
+ *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
+  goto __pyx_L0;
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":997
+ * 
+ * 
+ * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy datetime64 object
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":1007
+ * 
+ * 
+ * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ */
+
+static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
+  npy_timedelta __pyx_r;
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":1011
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ *     """
+ *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
+  goto __pyx_L0;
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":1007
+ * 
+ * 
+ * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":1014
+ * 
+ * 
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ */
+
+static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
+  NPY_DATETIMEUNIT __pyx_r;
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":1018
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ *     """
+ *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
+ */
+  __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
+  goto __pyx_L0;
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":1014
+ * 
+ * 
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
 /* "View.MemoryView":122
  *         cdef bint dtype_is_object
  * 
  *     def __cinit__(array self, tuple shape, Py_ssize_t itemsize, format not None,             # <<<<<<<<<<<<<<
  *                   mode="c", bint allocate_buffer=True):
  * 
  */
@@ -28102,15 +28292,15 @@
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {&__pyx_n_s_v, __pyx_k_v, sizeof(__pyx_k_v), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 36, __pyx_L1_error)
   __pyx_builtin_KeyboardInterrupt = __Pyx_GetBuiltinName(__pyx_n_s_KeyboardInterrupt); if (!__pyx_builtin_KeyboardInterrupt) __PYX_ERR(0, 148, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 884, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 945, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(2, 133, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(2, 148, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(2, 151, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(2, 2, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(2, 404, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(2, 613, __pyx_L1_error)
   __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(2, 832, __pyx_L1_error)
@@ -28130,33 +28320,33 @@
  *             for i in tbar:
  *                 if i <= lef_num:
  */
   __pyx_tuple_ = PyTuple_Pack(3, Py_None, Py_None, Py_None); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":884
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 884, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 945, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":890
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 890, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 951, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
   /* "View.MemoryView":133
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
@@ -28596,26 +28786,46 @@
   sizeof(PyTypeObject),
   #else
   sizeof(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 200, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 200, __pyx_L1_error)
   __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 223, __pyx_L1_error)
   __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 227, __pyx_L1_error)
   __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 239, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 771, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 773, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 775, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 777, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 779, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 781, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 783, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 785, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 787, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 789, __pyx_L1_error)
   __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 764, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 827, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("kgraph.utils.memory"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_6kgraph_5utils_6memory_Memory = __Pyx_ImportType(__pyx_t_1, "kgraph.utils.memory", "Memory", sizeof(struct __pyx_obj_6kgraph_5utils_6memory_Memory), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_6kgraph_5utils_6memory_Memory) __PYX_ERR(4, 70, __pyx_L1_error)
   __pyx_ptype_6kgraph_5utils_6memory_Data = __Pyx_ImportType(__pyx_t_1, "kgraph.utils.memory", "Data", sizeof(struct __pyx_obj_6kgraph_5utils_6memory_Data), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_6kgraph_5utils_6memory_Data) __PYX_ERR(4, 75, __pyx_L1_error)
```

### Comparing `kgraph-1.0.8/kgraph/utils/evaluation.pyx` & `kgraph-1.0.9/kgraph/utils/evaluation.pyx`

 * *Files identical despite different names*

### Comparing `kgraph-1.0.8/kgraph/utils/memory.cpp` & `kgraph-1.0.9/kgraph/utils/memory.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 /* Generated by Cython 0.29.28 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "C:\\ProgramData\\Miniconda3\\include\\Python.h",
-            "C:\\ProgramData\\Miniconda3\\include\\pythread.h"
+            "/home/long/miniconda3/include/python3.7m/Python.h",
+            "/home/long/miniconda3/include/python3.7m/pythread.h"
         ],
         "extra_compile_args": [
             "-std=c++11"
         ],
         "include_dirs": [
-            "C:\\ProgramData\\Miniconda3\\lib\\site-packages\\numpy\\core\\include",
-            "C:\\ProgramData\\Miniconda3\\include"
+            "/home/long/miniconda3/lib/python3.7/site-packages/numpy/core/include",
+            "/home/long/miniconda3/include/python3.7m"
         ],
         "language": "c++",
         "name": "kgraph.utils.memory",
         "sources": [
             "kgraph/utils/memory.pyx"
         ]
     },
@@ -937,17 +937,17 @@
 static int __pyx_lineno;
 static int __pyx_clineno = 0;
 static const char * __pyx_cfilenm= __FILE__;
 static const char *__pyx_filename;
 
 
 static const char *__pyx_f[] = {
-  "kgraph\\utils\\memory.pyx",
+  "kgraph/utils/memory.pyx",
   "stringsource",
-  "kgraph\\utils\\memory.pxd",
+  "kgraph/utils/memory.pxd",
   "type.pxd",
   "bool.pxd",
   "complex.pxd",
 };
 /* ForceInitThreads.proto */
 #ifndef __PYX_FORCE_INIT_THREADS
   #define __PYX_FORCE_INIT_THREADS 0
```

### Comparing `kgraph-1.0.8/kgraph/utils/memory.pxd` & `kgraph-1.0.9/kgraph/utils/memory.pxd`

 * *Files identical despite different names*

### Comparing `kgraph-1.0.8/kgraph/utils/memory.pyx` & `kgraph-1.0.9/kgraph/utils/memory.pyx`

 * *Files identical despite different names*

### Comparing `kgraph-1.0.8/kgraph/utils/read.cpp` & `kgraph-1.0.9/kgraph/utils/read.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 /* Generated by Cython 0.29.28 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "C:\\ProgramData\\Miniconda3\\include\\Python.h",
-            "C:\\ProgramData\\Miniconda3\\include\\pythread.h",
-            "C:\\ProgramData\\Miniconda3\\lib\\site-packages\\numpy\\core\\include\\numpy\\arrayobject.h",
-            "C:\\ProgramData\\Miniconda3\\lib\\site-packages\\numpy\\core\\include\\numpy\\ufuncobject.h"
+            "/home/long/miniconda3/include/python3.7m/Python.h",
+            "/home/long/miniconda3/include/python3.7m/pythread.h",
+            "/home/long/miniconda3/lib/python3.7/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/home/long/miniconda3/lib/python3.7/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/home/long/miniconda3/lib/python3.7/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/home/long/miniconda3/lib/python3.7/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/home/long/miniconda3/lib/python3.7/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "extra_compile_args": [
             "-std=c++11"
         ],
         "include_dirs": [
-            "C:\\ProgramData\\Miniconda3\\lib\\site-packages\\numpy\\core\\include",
-            "C:\\ProgramData\\Miniconda3\\include"
+            "/home/long/miniconda3/lib/python3.7/site-packages/numpy/core/include",
+            "/home/long/miniconda3/include/python3.7m"
         ],
         "language": "c++",
         "name": "kgraph.utils.read",
         "sources": [
             "kgraph/utils/read.pyx"
         ]
     },
@@ -721,14 +724,17 @@
 
 #define __PYX_HAVE__kgraph__utils__read
 #define __PYX_HAVE_API__kgraph__utils__read
 /* Early includes */
 #include <string.h>
 #include <stdio.h>
 #include "numpy/arrayobject.h"
+#include "numpy/ndarrayobject.h"
+#include "numpy/ndarraytypes.h"
+#include "numpy/arrayscalars.h"
 #include "numpy/ufuncobject.h"
 
     /* NumPy API declarations from "numpy/__init__.pxd" */
     
 #include <algorithm>
 #include <stdlib.h>
 #include "ios"
@@ -966,23 +972,23 @@
 #if CYTHON_CCOMPLEX && !defined(__cplusplus) && defined(__sun__) && defined(__GNUC__)
   #undef _Complex_I
   #define _Complex_I 1.0fj
 #endif
 
 
 static const char *__pyx_f[] = {
-  "kgraph\\utils\\read.pyx",
+  "kgraph/utils/read.pyx",
   "stringsource",
-  "kgraph\\utils\\read.pxd",
+  "kgraph/utils/read.pxd",
   "__init__.pxd",
   "array.pxd",
   "type.pxd",
   "bool.pxd",
   "complex.pxd",
-  "kgraph\\utils\\memory.pxd",
+  "kgraph/utils/memory.pxd",
 };
 /* MemviewSliceStruct.proto */
 struct __pyx_memoryview_obj;
 typedef struct {
   struct __pyx_memoryview_obj *memview;
   char *data;
   Py_ssize_t shape[8];
@@ -1085,195 +1091,195 @@
 #define __Pyx_PyGILState_Ensure PyGILState_Ensure
 #define __Pyx_PyGILState_Release PyGILState_Release
 #define __Pyx_FastGIL_Remember()
 #define __Pyx_FastGIL_Forget()
 #define __Pyx_FastGilFuncInit()
 
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":689
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":690
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":690
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":691
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":691
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":692
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":693
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":696
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":697
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":697
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":698
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":698
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":699
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":700
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":703
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":704
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":704
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":705
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":713
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":714
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":714
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":715
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":715
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":716
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":717
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":718
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":719
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":720
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":721
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":722
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":722
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":723
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":724
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":725
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":726
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1314,42 +1320,42 @@
 struct __pyx_obj_6kgraph_5utils_6memory_MemoryPool;
 struct __pyx_obj_6kgraph_5utils_4read_DataSet;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":728
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":729
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":730
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":730
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":732
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":733
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2900,14 +2906,24 @@
 /* Module declarations from 'numpy' */
 
 /* Module declarations from 'numpy' */
 static PyTypeObject *__pyx_ptype_5numpy_dtype = 0;
 static PyTypeObject *__pyx_ptype_5numpy_flatiter = 0;
 static PyTypeObject *__pyx_ptype_5numpy_broadcast = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ndarray = 0;
+static PyTypeObject *__pyx_ptype_5numpy_generic = 0;
+static PyTypeObject *__pyx_ptype_5numpy_number = 0;
+static PyTypeObject *__pyx_ptype_5numpy_integer = 0;
+static PyTypeObject *__pyx_ptype_5numpy_signedinteger = 0;
+static PyTypeObject *__pyx_ptype_5numpy_unsignedinteger = 0;
+static PyTypeObject *__pyx_ptype_5numpy_inexact = 0;
+static PyTypeObject *__pyx_ptype_5numpy_floating = 0;
+static PyTypeObject *__pyx_ptype_5numpy_complexfloating = 0;
+static PyTypeObject *__pyx_ptype_5numpy_flexible = 0;
+static PyTypeObject *__pyx_ptype_5numpy_character = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ufunc = 0;
 
 /* Module declarations from 'libcpp' */
 
 /* Module declarations from 'libcpp.algorithm' */
 
 /* Module declarations from 'libc.stdlib' */
@@ -3157,31 +3173,33 @@
 static const char __pyx_k_pyx_unpickle_Enum[] = "__pyx_unpickle_Enum";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_strided_and_direct[] = "<strided and direct>";
 static const char __pyx_k_strided_and_indirect[] = "<strided and indirect>";
 static const char __pyx_k_contiguous_and_direct[] = "<contiguous and direct>";
 static const char __pyx_k_entity2id_no_sort_txt[] = "entity2id_no_sort.txt";
 static const char __pyx_k_entity2id_on_sort_txt[] = "entity2id_on_sort.txt";
-static const char __pyx_k_kgraph_utils_read_pyx[] = "kgraph\\utils\\read.pyx";
+static const char __pyx_k_kgraph_utils_read_pyx[] = "kgraph/utils/read.pyx";
 static const char __pyx_k_MemoryView_of_r_object[] = "<MemoryView of %r object>";
 static const char __pyx_k_MemoryView_of_r_at_0x_x[] = "<MemoryView of %r at 0x%x>";
 static const char __pyx_k_contiguous_and_indirect[] = "<contiguous and indirect>";
 static const char __pyx_k_relation2id_no_sort_txt[] = "relation2id_no_sort.txt";
 static const char __pyx_k_relation2id_on_sort_txt[] = "relation2id_on_sort.txt";
 static const char __pyx_k_Cannot_index_with_type_s[] = "Cannot index with type '%s'";
 static const char __pyx_k_Invalid_shape_in_axis_d_d[] = "Invalid shape in axis %d: %d.";
 static const char __pyx_k_calculate_train_data_size[] = "__calculate_train_data_size";
 static const char __pyx_k_itemsize_0_for_cython_array[] = "itemsize <= 0 for cython.array";
 static const char __pyx_k_unable_to_allocate_array_data[] = "unable to allocate array data.";
 static const char __pyx_k_strided_and_direct_or_indirect[] = "<strided and direct or indirect>";
+static const char __pyx_k_TODO_Generate_the_triple_sample[] = "\n        TODO: Generate the triple samples for training.\n        return triples, labels\n\n        eg.:\n        >>>data = FB15k()\n        >>>samples, labels = data.get_item_triple(1)\n\n        samples:[[[12, 1, 4]]] labels:[[0]]\n\n        eg.:\n        >>>data = FB15k()\n        >>>data.num_neg = 4\n        >>>samples, labels = data.get_item_triple(1)\n\n        samples:[[[12, 1, 5], [12, 1, 138], [0, 1, 5], [12, 1, 7], [12, 1, 4]]]  labels:[[1, 1, -1, 1, 0]]\n\n        In labels, 1 means that replace the head entity, and -1 means that replace the tail entity, and 0 defines the original triple.\n        ";
 static const char __pyx_k_numpy_core_multiarray_failed_to[] = "numpy.core.multiarray failed to import";
 static const char __pyx_k_Buffer_view_does_not_expose_stri[] = "Buffer view does not expose strides";
 static const char __pyx_k_Can_only_create_a_buffer_that_is[] = "Can only create a buffer that is contiguous in memory.";
 static const char __pyx_k_Cannot_assign_to_read_only_memor[] = "Cannot assign to read-only memoryview";
 static const char __pyx_k_Cannot_create_writable_memory_vi[] = "Cannot create writable memory view from read-only memoryview";
+static const char __pyx_k_DataSet_get_item_triple_line_805[] = "DataSet.get_item_triple (line 805)";
 static const char __pyx_k_Empty_shape_tuple_for_cython_arr[] = "Empty shape tuple for cython.array";
 static const char __pyx_k_Incompatible_checksums_s_vs_0xb0[] = "Incompatible checksums (%s vs 0xb068931 = (name))";
 static const char __pyx_k_Indirect_dimensions_not_supporte[] = "Indirect dimensions not supported";
 static const char __pyx_k_Invalid_mode_expected_c_or_fortr[] = "Invalid mode, expected 'c' or 'fortran', got %s";
 static const char __pyx_k_Out_of_bounds_on_buffer_access_a[] = "Out of bounds on buffer access (axis %d)";
 static const char __pyx_k_Unable_to_convert_item_to_object[] = "Unable to convert item to object";
 static const char __pyx_k_got_differing_extents_in_dimensi[] = "got differing extents in dimension %d (got %d and %d)";
@@ -3193,14 +3211,15 @@
 static PyObject *__pyx_n_s_ASCII;
 static PyObject *__pyx_kp_s_Buffer_view_does_not_expose_stri;
 static PyObject *__pyx_kp_s_Can_only_create_a_buffer_that_is;
 static PyObject *__pyx_kp_s_Cannot_assign_to_read_only_memor;
 static PyObject *__pyx_kp_s_Cannot_create_writable_memory_vi;
 static PyObject *__pyx_kp_s_Cannot_index_with_type_s;
 static PyObject *__pyx_n_s_DataSet;
+static PyObject *__pyx_kp_u_DataSet_get_item_triple_line_805;
 static PyObject *__pyx_n_s_Ellipsis;
 static PyObject *__pyx_kp_s_Empty_shape_tuple_for_cython_arr;
 static PyObject *__pyx_n_s_ImportError;
 static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0xb0;
 static PyObject *__pyx_n_s_IndexError;
 static PyObject *__pyx_kp_s_Indirect_dimensions_not_supporte;
 static PyObject *__pyx_kp_s_Invalid_mode_expected_c_or_fortr;
@@ -3208,14 +3227,15 @@
 static PyObject *__pyx_n_s_MemoryError;
 static PyObject *__pyx_kp_s_MemoryView_of_r_at_0x_x;
 static PyObject *__pyx_kp_s_MemoryView_of_r_object;
 static PyObject *__pyx_n_b_O;
 static PyObject *__pyx_kp_s_Out_of_bounds_on_buffer_access_a;
 static PyObject *__pyx_n_s_PickleError;
 static PyObject *__pyx_kp_b_T;
+static PyObject *__pyx_kp_u_TODO_Generate_the_triple_sample;
 static PyObject *__pyx_n_s_TypeError;
 static PyObject *__pyx_kp_s_Unable_to_convert_item_to_object;
 static PyObject *__pyx_n_s_ValueError;
 static PyObject *__pyx_n_s_View_MemoryView;
 static PyObject *__pyx_kp_b__26;
 static PyObject *__pyx_kp_b__27;
 static PyObject *__pyx_kp_b__28;
@@ -9266,20 +9286,21 @@
   return __pyx_r;
 }
 
 /* "kgraph/utils/read.pyx":574
  *         self.__calculate_train_data_size()
  * 
  *     def getTrain(self):             # <<<<<<<<<<<<<<
- *         # global train_data
- *         return getDataFromCache_c(&(self.train_data_ptr))
+ *         """
+ *         return the array of train data.
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_6kgraph_5utils_4read_7DataSet_5getTrain(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_6kgraph_5utils_4read_7DataSet_4getTrain[] = "\n        return the array of train data.\n        ";
 static PyObject *__pyx_pw_6kgraph_5utils_4read_7DataSet_5getTrain(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("getTrain (wrapper)", 0);
   __pyx_r = __pyx_pf_6kgraph_5utils_4read_7DataSet_4getTrain(((struct __pyx_obj_6kgraph_5utils_4read_DataSet *)__pyx_v_self));
 
   /* function exit code */
@@ -9292,57 +9313,58 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("getTrain", 0);
 
-  /* "kgraph/utils/read.pyx":576
- *     def getTrain(self):
+  /* "kgraph/utils/read.pyx":579
+ *         """
  *         # global train_data
  *         return getDataFromCache_c(&(self.train_data_ptr))             # <<<<<<<<<<<<<<
  * 
  *     def getValid(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = ((PyObject *)__pyx_f_6kgraph_5utils_4read_getDataFromCache_c((&__pyx_v_self->train_data_ptr))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 576, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__pyx_f_6kgraph_5utils_4read_getDataFromCache_c((&__pyx_v_self->train_data_ptr))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 579, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "kgraph/utils/read.pyx":574
  *         self.__calculate_train_data_size()
  * 
  *     def getTrain(self):             # <<<<<<<<<<<<<<
- *         # global train_data
- *         return getDataFromCache_c(&(self.train_data_ptr))
+ *         """
+ *         return the array of train data.
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("kgraph.utils.read.DataSet.getTrain", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kgraph/utils/read.pyx":578
+/* "kgraph/utils/read.pyx":581
  *         return getDataFromCache_c(&(self.train_data_ptr))
  * 
  *     def getValid(self):             # <<<<<<<<<<<<<<
- *         # global valid_data
- *         return getDataFromCache_c(&(self.valid_data_ptr))
+ *         """
+ *         return the array of valid data.
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_6kgraph_5utils_4read_7DataSet_7getValid(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_6kgraph_5utils_4read_7DataSet_6getValid[] = "\n        return the array of valid data.\n        ";
 static PyObject *__pyx_pw_6kgraph_5utils_4read_7DataSet_7getValid(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("getValid (wrapper)", 0);
   __pyx_r = __pyx_pf_6kgraph_5utils_4read_7DataSet_6getValid(((struct __pyx_obj_6kgraph_5utils_4read_DataSet *)__pyx_v_self));
 
   /* function exit code */
@@ -9355,57 +9377,58 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("getValid", 0);
 
-  /* "kgraph/utils/read.pyx":580
- *     def getValid(self):
+  /* "kgraph/utils/read.pyx":586
+ *         """
  *         # global valid_data
  *         return getDataFromCache_c(&(self.valid_data_ptr))             # <<<<<<<<<<<<<<
  * 
  *     def getTest(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = ((PyObject *)__pyx_f_6kgraph_5utils_4read_getDataFromCache_c((&__pyx_v_self->valid_data_ptr))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 580, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__pyx_f_6kgraph_5utils_4read_getDataFromCache_c((&__pyx_v_self->valid_data_ptr))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 586, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "kgraph/utils/read.pyx":578
+  /* "kgraph/utils/read.pyx":581
  *         return getDataFromCache_c(&(self.train_data_ptr))
  * 
  *     def getValid(self):             # <<<<<<<<<<<<<<
- *         # global valid_data
- *         return getDataFromCache_c(&(self.valid_data_ptr))
+ *         """
+ *         return the array of valid data.
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("kgraph.utils.read.DataSet.getValid", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kgraph/utils/read.pyx":582
+/* "kgraph/utils/read.pyx":588
  *         return getDataFromCache_c(&(self.valid_data_ptr))
  * 
  *     def getTest(self):             # <<<<<<<<<<<<<<
- *         # global test_data
- *         return getDataFromCache_c(&(self.test_data_ptr))
+ *         """
+ *         return the array of test data.
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_6kgraph_5utils_4read_7DataSet_9getTest(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_6kgraph_5utils_4read_7DataSet_8getTest[] = "\n        return the array of test data.\n        ";
 static PyObject *__pyx_pw_6kgraph_5utils_4read_7DataSet_9getTest(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("getTest (wrapper)", 0);
   __pyx_r = __pyx_pf_6kgraph_5utils_4read_7DataSet_8getTest(((struct __pyx_obj_6kgraph_5utils_4read_DataSet *)__pyx_v_self));
 
   /* function exit code */
@@ -9418,57 +9441,58 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("getTest", 0);
 
-  /* "kgraph/utils/read.pyx":584
- *     def getTest(self):
+  /* "kgraph/utils/read.pyx":593
+ *         """
  *         # global test_data
  *         return getDataFromCache_c(&(self.test_data_ptr))             # <<<<<<<<<<<<<<
  * 
  *     def getAll(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = ((PyObject *)__pyx_f_6kgraph_5utils_4read_getDataFromCache_c((&__pyx_v_self->test_data_ptr))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 584, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__pyx_f_6kgraph_5utils_4read_getDataFromCache_c((&__pyx_v_self->test_data_ptr))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 593, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "kgraph/utils/read.pyx":582
+  /* "kgraph/utils/read.pyx":588
  *         return getDataFromCache_c(&(self.valid_data_ptr))
  * 
  *     def getTest(self):             # <<<<<<<<<<<<<<
- *         # global test_data
- *         return getDataFromCache_c(&(self.test_data_ptr))
+ *         """
+ *         return the array of test data.
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("kgraph.utils.read.DataSet.getTest", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kgraph/utils/read.pyx":586
+/* "kgraph/utils/read.pyx":595
  *         return getDataFromCache_c(&(self.test_data_ptr))
  * 
  *     def getAll(self):             # <<<<<<<<<<<<<<
- *         # global all_triples
- *         return getDataFromCache_c(&(self.all_triples_ptr))
+ *         """
+ *         return the array of all data.
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_6kgraph_5utils_4read_7DataSet_11getAll(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_6kgraph_5utils_4read_7DataSet_10getAll[] = "\n        return the array of all data.\n        ";
 static PyObject *__pyx_pw_6kgraph_5utils_4read_7DataSet_11getAll(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("getAll (wrapper)", 0);
   __pyx_r = __pyx_pf_6kgraph_5utils_4read_7DataSet_10getAll(((struct __pyx_obj_6kgraph_5utils_4read_DataSet *)__pyx_v_self));
 
   /* function exit code */
@@ -9481,48 +9505,48 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("getAll", 0);
 
-  /* "kgraph/utils/read.pyx":588
- *     def getAll(self):
+  /* "kgraph/utils/read.pyx":600
+ *         """
  *         # global all_triples
  *         return getDataFromCache_c(&(self.all_triples_ptr))             # <<<<<<<<<<<<<<
  * 
  *     def resetPosAndNegTest(self, flag=False):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = ((PyObject *)__pyx_f_6kgraph_5utils_4read_getDataFromCache_c((&__pyx_v_self->all_triples_ptr))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 588, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__pyx_f_6kgraph_5utils_4read_getDataFromCache_c((&__pyx_v_self->all_triples_ptr))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 600, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "kgraph/utils/read.pyx":586
+  /* "kgraph/utils/read.pyx":595
  *         return getDataFromCache_c(&(self.test_data_ptr))
  * 
  *     def getAll(self):             # <<<<<<<<<<<<<<
- *         # global all_triples
- *         return getDataFromCache_c(&(self.all_triples_ptr))
+ *         """
+ *         return the array of all data.
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("kgraph.utils.read.DataSet.getAll", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kgraph/utils/read.pyx":590
+/* "kgraph/utils/read.pyx":602
  *         return getDataFromCache_c(&(self.all_triples_ptr))
  * 
  *     def resetPosAndNegTest(self, flag=False):             # <<<<<<<<<<<<<<
  *         test_array = self.getTest()
  * 
  */
 
@@ -9554,29 +9578,29 @@
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_flag);
           if (value) { values[0] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "resetPosAndNegTest") < 0)) __PYX_ERR(0, 590, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "resetPosAndNegTest") < 0)) __PYX_ERR(0, 602, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_flag = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("resetPosAndNegTest", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 590, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("resetPosAndNegTest", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 602, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("kgraph.utils.read.DataSet.resetPosAndNegTest", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6kgraph_5utils_4read_7DataSet_12resetPosAndNegTest(((struct __pyx_obj_6kgraph_5utils_4read_DataSet *)__pyx_v_self), __pyx_v_flag);
 
@@ -9605,358 +9629,358 @@
   PyObject *__pyx_t_7 = NULL;
   __Pyx_memviewslice __pyx_t_8 = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("resetPosAndNegTest", 0);
 
-  /* "kgraph/utils/read.pyx":591
+  /* "kgraph/utils/read.pyx":603
  * 
  *     def resetPosAndNegTest(self, flag=False):
  *         test_array = self.getTest()             # <<<<<<<<<<<<<<
  * 
  *         if flag:
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_getTest); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 591, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_getTest); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 603, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 591, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 603, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_test_array = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "kgraph/utils/read.pyx":593
+  /* "kgraph/utils/read.pyx":605
  *         test_array = self.getTest()
  * 
  *         if flag:             # <<<<<<<<<<<<<<
  *             idx = range(len(test_array) // 2)
  *             pos_idx = [2 * x for x in idx]
  */
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_flag); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 593, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_flag); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 605, __pyx_L1_error)
   if (__pyx_t_4) {
 
-    /* "kgraph/utils/read.pyx":594
+    /* "kgraph/utils/read.pyx":606
  * 
  *         if flag:
  *             idx = range(len(test_array) // 2)             # <<<<<<<<<<<<<<
  *             pos_idx = [2 * x for x in idx]
  *             neg_idx = [2 * x + 1 for x in idx]
  */
-    __pyx_t_5 = PyObject_Length(__pyx_v_test_array); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 594, __pyx_L1_error)
-    __pyx_t_1 = PyInt_FromSsize_t(__Pyx_div_Py_ssize_t(__pyx_t_5, 2)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 594, __pyx_L1_error)
+    __pyx_t_5 = PyObject_Length(__pyx_v_test_array); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 606, __pyx_L1_error)
+    __pyx_t_1 = PyInt_FromSsize_t(__Pyx_div_Py_ssize_t(__pyx_t_5, 2)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 606, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 594, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 606, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_v_idx = __pyx_t_2;
     __pyx_t_2 = 0;
 
-    /* "kgraph/utils/read.pyx":595
+    /* "kgraph/utils/read.pyx":607
  *         if flag:
  *             idx = range(len(test_array) // 2)
  *             pos_idx = [2 * x for x in idx]             # <<<<<<<<<<<<<<
  *             neg_idx = [2 * x + 1 for x in idx]
  *             pos_test_array = test_array[pos_idx, :]
  */
     { /* enter inner scope */
-      __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 595, __pyx_L6_error)
+      __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 607, __pyx_L6_error)
       __Pyx_GOTREF(__pyx_t_2);
       if (likely(PyList_CheckExact(__pyx_v_idx)) || PyTuple_CheckExact(__pyx_v_idx)) {
         __pyx_t_1 = __pyx_v_idx; __Pyx_INCREF(__pyx_t_1); __pyx_t_5 = 0;
         __pyx_t_6 = NULL;
       } else {
-        __pyx_t_5 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_idx); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 595, __pyx_L6_error)
+        __pyx_t_5 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_idx); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 607, __pyx_L6_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_6 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 595, __pyx_L6_error)
+        __pyx_t_6 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 607, __pyx_L6_error)
       }
       for (;;) {
         if (likely(!__pyx_t_6)) {
           if (likely(PyList_CheckExact(__pyx_t_1))) {
             if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_1)) break;
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_3 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_3); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 595, __pyx_L6_error)
+            __pyx_t_3 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_3); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 607, __pyx_L6_error)
             #else
-            __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 595, __pyx_L6_error)
+            __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 607, __pyx_L6_error)
             __Pyx_GOTREF(__pyx_t_3);
             #endif
           } else {
             if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_3); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 595, __pyx_L6_error)
+            __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_3); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 607, __pyx_L6_error)
             #else
-            __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 595, __pyx_L6_error)
+            __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 607, __pyx_L6_error)
             __Pyx_GOTREF(__pyx_t_3);
             #endif
           }
         } else {
           __pyx_t_3 = __pyx_t_6(__pyx_t_1);
           if (unlikely(!__pyx_t_3)) {
             PyObject* exc_type = PyErr_Occurred();
             if (exc_type) {
               if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-              else __PYX_ERR(0, 595, __pyx_L6_error)
+              else __PYX_ERR(0, 607, __pyx_L6_error)
             }
             break;
           }
           __Pyx_GOTREF(__pyx_t_3);
         }
         __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_x, __pyx_t_3);
         __pyx_t_3 = 0;
-        __pyx_t_3 = PyNumber_Multiply(__pyx_int_2, __pyx_7genexpr__pyx_v_x); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 595, __pyx_L6_error)
+        __pyx_t_3 = PyNumber_Multiply(__pyx_int_2, __pyx_7genexpr__pyx_v_x); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 607, __pyx_L6_error)
         __Pyx_GOTREF(__pyx_t_3);
-        if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_3))) __PYX_ERR(0, 595, __pyx_L6_error)
+        if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_3))) __PYX_ERR(0, 607, __pyx_L6_error)
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       }
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_XDECREF(__pyx_7genexpr__pyx_v_x); __pyx_7genexpr__pyx_v_x = 0;
       goto __pyx_L9_exit_scope;
       __pyx_L6_error:;
       __Pyx_XDECREF(__pyx_7genexpr__pyx_v_x); __pyx_7genexpr__pyx_v_x = 0;
       goto __pyx_L1_error;
       __pyx_L9_exit_scope:;
     } /* exit inner scope */
     __pyx_v_pos_idx = ((PyObject*)__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "kgraph/utils/read.pyx":596
+    /* "kgraph/utils/read.pyx":608
  *             idx = range(len(test_array) // 2)
  *             pos_idx = [2 * x for x in idx]
  *             neg_idx = [2 * x + 1 for x in idx]             # <<<<<<<<<<<<<<
  *             pos_test_array = test_array[pos_idx, :]
  *             neg_test_array = test_array[neg_idx, :]
  */
     { /* enter inner scope */
-      __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 596, __pyx_L12_error)
+      __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 608, __pyx_L12_error)
       __Pyx_GOTREF(__pyx_t_2);
       if (likely(PyList_CheckExact(__pyx_v_idx)) || PyTuple_CheckExact(__pyx_v_idx)) {
         __pyx_t_1 = __pyx_v_idx; __Pyx_INCREF(__pyx_t_1); __pyx_t_5 = 0;
         __pyx_t_6 = NULL;
       } else {
-        __pyx_t_5 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_idx); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 596, __pyx_L12_error)
+        __pyx_t_5 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_idx); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 608, __pyx_L12_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_6 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 596, __pyx_L12_error)
+        __pyx_t_6 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 608, __pyx_L12_error)
       }
       for (;;) {
         if (likely(!__pyx_t_6)) {
           if (likely(PyList_CheckExact(__pyx_t_1))) {
             if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_1)) break;
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_3 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_3); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 596, __pyx_L12_error)
+            __pyx_t_3 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_3); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 608, __pyx_L12_error)
             #else
-            __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 596, __pyx_L12_error)
+            __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 608, __pyx_L12_error)
             __Pyx_GOTREF(__pyx_t_3);
             #endif
           } else {
             if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_3); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 596, __pyx_L12_error)
+            __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_3); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 608, __pyx_L12_error)
             #else
-            __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 596, __pyx_L12_error)
+            __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 608, __pyx_L12_error)
             __Pyx_GOTREF(__pyx_t_3);
             #endif
           }
         } else {
           __pyx_t_3 = __pyx_t_6(__pyx_t_1);
           if (unlikely(!__pyx_t_3)) {
             PyObject* exc_type = PyErr_Occurred();
             if (exc_type) {
               if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-              else __PYX_ERR(0, 596, __pyx_L12_error)
+              else __PYX_ERR(0, 608, __pyx_L12_error)
             }
             break;
           }
           __Pyx_GOTREF(__pyx_t_3);
         }
         __Pyx_XDECREF_SET(__pyx_8genexpr1__pyx_v_x, __pyx_t_3);
         __pyx_t_3 = 0;
-        __pyx_t_3 = PyNumber_Multiply(__pyx_int_2, __pyx_8genexpr1__pyx_v_x); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 596, __pyx_L12_error)
+        __pyx_t_3 = PyNumber_Multiply(__pyx_int_2, __pyx_8genexpr1__pyx_v_x); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 608, __pyx_L12_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_t_3, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 596, __pyx_L12_error)
+        __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_t_3, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 608, __pyx_L12_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_7))) __PYX_ERR(0, 596, __pyx_L12_error)
+        if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_7))) __PYX_ERR(0, 608, __pyx_L12_error)
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       }
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_x); __pyx_8genexpr1__pyx_v_x = 0;
       goto __pyx_L15_exit_scope;
       __pyx_L12_error:;
       __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_x); __pyx_8genexpr1__pyx_v_x = 0;
       goto __pyx_L1_error;
       __pyx_L15_exit_scope:;
     } /* exit inner scope */
     __pyx_v_neg_idx = ((PyObject*)__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "kgraph/utils/read.pyx":597
+    /* "kgraph/utils/read.pyx":609
  *             pos_idx = [2 * x for x in idx]
  *             neg_idx = [2 * x + 1 for x in idx]
  *             pos_test_array = test_array[pos_idx, :]             # <<<<<<<<<<<<<<
  *             neg_test_array = test_array[neg_idx, :]
  *             putTestInCache_c(&(self.test_pos_data_ptr), pos_test_array, self.num_ent, self.num_rel, self.tmp_memory_pool)
  */
-    __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 597, __pyx_L1_error)
+    __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 609, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_INCREF(__pyx_v_pos_idx);
     __Pyx_GIVEREF(__pyx_v_pos_idx);
     PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_pos_idx);
     __Pyx_INCREF(__pyx_slice_);
     __Pyx_GIVEREF(__pyx_slice_);
     PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_slice_);
-    __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_test_array, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 597, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_test_array, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 609, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_v_pos_test_array = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "kgraph/utils/read.pyx":598
+    /* "kgraph/utils/read.pyx":610
  *             neg_idx = [2 * x + 1 for x in idx]
  *             pos_test_array = test_array[pos_idx, :]
  *             neg_test_array = test_array[neg_idx, :]             # <<<<<<<<<<<<<<
  *             putTestInCache_c(&(self.test_pos_data_ptr), pos_test_array, self.num_ent, self.num_rel, self.tmp_memory_pool)
  *             putTestInCache_c(&(self.test_neg_data_ptr), neg_test_array, self.num_ent, self.num_rel, self.tmp_memory_pool)
  */
-    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 598, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 610, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_v_neg_idx);
     __Pyx_GIVEREF(__pyx_v_neg_idx);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_neg_idx);
     __Pyx_INCREF(__pyx_slice_);
     __Pyx_GIVEREF(__pyx_slice_);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_slice_);
-    __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_v_test_array, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 598, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_v_test_array, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 610, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_v_neg_test_array = __pyx_t_2;
     __pyx_t_2 = 0;
 
-    /* "kgraph/utils/read.pyx":599
+    /* "kgraph/utils/read.pyx":611
  *             pos_test_array = test_array[pos_idx, :]
  *             neg_test_array = test_array[neg_idx, :]
  *             putTestInCache_c(&(self.test_pos_data_ptr), pos_test_array, self.num_ent, self.num_rel, self.tmp_memory_pool)             # <<<<<<<<<<<<<<
  *             putTestInCache_c(&(self.test_neg_data_ptr), neg_test_array, self.num_ent, self.num_rel, self.tmp_memory_pool)
  *             putTestInCache_c(&(self.test_data_ptr), pos_test_array, self.num_ent, self.num_rel, self.tmp_memory_pool)
  */
-    __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int(__pyx_v_pos_test_array, PyBUF_WRITABLE); if (unlikely(!__pyx_t_8.memview)) __PYX_ERR(0, 599, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int(__pyx_v_pos_test_array, PyBUF_WRITABLE); if (unlikely(!__pyx_t_8.memview)) __PYX_ERR(0, 611, __pyx_L1_error)
     __pyx_t_2 = ((PyObject *)__pyx_v_self->tmp_memory_pool);
     __Pyx_INCREF(__pyx_t_2);
     __pyx_f_6kgraph_5utils_4read_putTestInCache_c((&__pyx_v_self->test_pos_data_ptr), __pyx_t_8, __pyx_v_self->num_ent, __pyx_v_self->num_rel, ((struct __pyx_obj_6kgraph_5utils_6memory_MemoryPool *)__pyx_t_2));
     __PYX_XDEC_MEMVIEW(&__pyx_t_8, 1);
     __pyx_t_8.memview = NULL;
     __pyx_t_8.data = NULL;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "kgraph/utils/read.pyx":600
+    /* "kgraph/utils/read.pyx":612
  *             neg_test_array = test_array[neg_idx, :]
  *             putTestInCache_c(&(self.test_pos_data_ptr), pos_test_array, self.num_ent, self.num_rel, self.tmp_memory_pool)
  *             putTestInCache_c(&(self.test_neg_data_ptr), neg_test_array, self.num_ent, self.num_rel, self.tmp_memory_pool)             # <<<<<<<<<<<<<<
  *             putTestInCache_c(&(self.test_data_ptr), pos_test_array, self.num_ent, self.num_rel, self.tmp_memory_pool)
  *             self.triple_generate_negative_for_classification = 1
  */
-    __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int(__pyx_v_neg_test_array, PyBUF_WRITABLE); if (unlikely(!__pyx_t_8.memview)) __PYX_ERR(0, 600, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int(__pyx_v_neg_test_array, PyBUF_WRITABLE); if (unlikely(!__pyx_t_8.memview)) __PYX_ERR(0, 612, __pyx_L1_error)
     __pyx_t_2 = ((PyObject *)__pyx_v_self->tmp_memory_pool);
     __Pyx_INCREF(__pyx_t_2);
     __pyx_f_6kgraph_5utils_4read_putTestInCache_c((&__pyx_v_self->test_neg_data_ptr), __pyx_t_8, __pyx_v_self->num_ent, __pyx_v_self->num_rel, ((struct __pyx_obj_6kgraph_5utils_6memory_MemoryPool *)__pyx_t_2));
     __PYX_XDEC_MEMVIEW(&__pyx_t_8, 1);
     __pyx_t_8.memview = NULL;
     __pyx_t_8.data = NULL;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "kgraph/utils/read.pyx":601
+    /* "kgraph/utils/read.pyx":613
  *             putTestInCache_c(&(self.test_pos_data_ptr), pos_test_array, self.num_ent, self.num_rel, self.tmp_memory_pool)
  *             putTestInCache_c(&(self.test_neg_data_ptr), neg_test_array, self.num_ent, self.num_rel, self.tmp_memory_pool)
  *             putTestInCache_c(&(self.test_data_ptr), pos_test_array, self.num_ent, self.num_rel, self.tmp_memory_pool)             # <<<<<<<<<<<<<<
  *             self.triple_generate_negative_for_classification = 1
  *         else:
  */
-    __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int(__pyx_v_pos_test_array, PyBUF_WRITABLE); if (unlikely(!__pyx_t_8.memview)) __PYX_ERR(0, 601, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int(__pyx_v_pos_test_array, PyBUF_WRITABLE); if (unlikely(!__pyx_t_8.memview)) __PYX_ERR(0, 613, __pyx_L1_error)
     __pyx_t_2 = ((PyObject *)__pyx_v_self->tmp_memory_pool);
     __Pyx_INCREF(__pyx_t_2);
     __pyx_f_6kgraph_5utils_4read_putTestInCache_c((&__pyx_v_self->test_data_ptr), __pyx_t_8, __pyx_v_self->num_ent, __pyx_v_self->num_rel, ((struct __pyx_obj_6kgraph_5utils_6memory_MemoryPool *)__pyx_t_2));
     __PYX_XDEC_MEMVIEW(&__pyx_t_8, 1);
     __pyx_t_8.memview = NULL;
     __pyx_t_8.data = NULL;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "kgraph/utils/read.pyx":602
+    /* "kgraph/utils/read.pyx":614
  *             putTestInCache_c(&(self.test_neg_data_ptr), neg_test_array, self.num_ent, self.num_rel, self.tmp_memory_pool)
  *             putTestInCache_c(&(self.test_data_ptr), pos_test_array, self.num_ent, self.num_rel, self.tmp_memory_pool)
  *             self.triple_generate_negative_for_classification = 1             # <<<<<<<<<<<<<<
  *         else:
  *             putTestInCache_c(&(self.test_pos_data_ptr), test_array, self.num_ent, self.num_rel, self.tmp_memory_pool)
  */
     __pyx_v_self->triple_generate_negative_for_classification = 1;
 
-    /* "kgraph/utils/read.pyx":593
+    /* "kgraph/utils/read.pyx":605
  *         test_array = self.getTest()
  * 
  *         if flag:             # <<<<<<<<<<<<<<
  *             idx = range(len(test_array) // 2)
  *             pos_idx = [2 * x for x in idx]
  */
     goto __pyx_L3;
   }
 
-  /* "kgraph/utils/read.pyx":604
+  /* "kgraph/utils/read.pyx":616
  *             self.triple_generate_negative_for_classification = 1
  *         else:
  *             putTestInCache_c(&(self.test_pos_data_ptr), test_array, self.num_ent, self.num_rel, self.tmp_memory_pool)             # <<<<<<<<<<<<<<
  *             putTestInCache_c(&(self.test_neg_data_ptr), test_array, self.num_ent, self.num_rel, self.tmp_memory_pool)
  *             self.triple_generate_negative_for_classification = 0
  */
   /*else*/ {
-    __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int(__pyx_v_test_array, PyBUF_WRITABLE); if (unlikely(!__pyx_t_8.memview)) __PYX_ERR(0, 604, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int(__pyx_v_test_array, PyBUF_WRITABLE); if (unlikely(!__pyx_t_8.memview)) __PYX_ERR(0, 616, __pyx_L1_error)
     __pyx_t_2 = ((PyObject *)__pyx_v_self->tmp_memory_pool);
     __Pyx_INCREF(__pyx_t_2);
     __pyx_f_6kgraph_5utils_4read_putTestInCache_c((&__pyx_v_self->test_pos_data_ptr), __pyx_t_8, __pyx_v_self->num_ent, __pyx_v_self->num_rel, ((struct __pyx_obj_6kgraph_5utils_6memory_MemoryPool *)__pyx_t_2));
     __PYX_XDEC_MEMVIEW(&__pyx_t_8, 1);
     __pyx_t_8.memview = NULL;
     __pyx_t_8.data = NULL;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "kgraph/utils/read.pyx":605
+    /* "kgraph/utils/read.pyx":617
  *         else:
  *             putTestInCache_c(&(self.test_pos_data_ptr), test_array, self.num_ent, self.num_rel, self.tmp_memory_pool)
  *             putTestInCache_c(&(self.test_neg_data_ptr), test_array, self.num_ent, self.num_rel, self.tmp_memory_pool)             # <<<<<<<<<<<<<<
  *             self.triple_generate_negative_for_classification = 0
  * 
  */
-    __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int(__pyx_v_test_array, PyBUF_WRITABLE); if (unlikely(!__pyx_t_8.memview)) __PYX_ERR(0, 605, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int(__pyx_v_test_array, PyBUF_WRITABLE); if (unlikely(!__pyx_t_8.memview)) __PYX_ERR(0, 617, __pyx_L1_error)
     __pyx_t_2 = ((PyObject *)__pyx_v_self->tmp_memory_pool);
     __Pyx_INCREF(__pyx_t_2);
     __pyx_f_6kgraph_5utils_4read_putTestInCache_c((&__pyx_v_self->test_neg_data_ptr), __pyx_t_8, __pyx_v_self->num_ent, __pyx_v_self->num_rel, ((struct __pyx_obj_6kgraph_5utils_6memory_MemoryPool *)__pyx_t_2));
     __PYX_XDEC_MEMVIEW(&__pyx_t_8, 1);
     __pyx_t_8.memview = NULL;
     __pyx_t_8.data = NULL;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "kgraph/utils/read.pyx":606
+    /* "kgraph/utils/read.pyx":618
  *             putTestInCache_c(&(self.test_pos_data_ptr), test_array, self.num_ent, self.num_rel, self.tmp_memory_pool)
  *             putTestInCache_c(&(self.test_neg_data_ptr), test_array, self.num_ent, self.num_rel, self.tmp_memory_pool)
  *             self.triple_generate_negative_for_classification = 0             # <<<<<<<<<<<<<<
  * 
  *     def resetPosAndNegValid(self, flag=False):
  */
     __pyx_v_self->triple_generate_negative_for_classification = 0;
   }
   __pyx_L3:;
 
-  /* "kgraph/utils/read.pyx":590
+  /* "kgraph/utils/read.pyx":602
  *         return getDataFromCache_c(&(self.all_triples_ptr))
  * 
  *     def resetPosAndNegTest(self, flag=False):             # <<<<<<<<<<<<<<
  *         test_array = self.getTest()
  * 
  */
 
@@ -9981,15 +10005,15 @@
   __Pyx_XDECREF(__pyx_7genexpr__pyx_v_x);
   __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_x);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kgraph/utils/read.pyx":608
+/* "kgraph/utils/read.pyx":620
  *             self.triple_generate_negative_for_classification = 0
  * 
  *     def resetPosAndNegValid(self, flag=False):             # <<<<<<<<<<<<<<
  *         valid_array = self.getValid()
  * 
  */
 
@@ -10021,29 +10045,29 @@
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_flag);
           if (value) { values[0] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "resetPosAndNegValid") < 0)) __PYX_ERR(0, 608, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "resetPosAndNegValid") < 0)) __PYX_ERR(0, 620, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_flag = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("resetPosAndNegValid", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 608, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("resetPosAndNegValid", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 620, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("kgraph.utils.read.DataSet.resetPosAndNegValid", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6kgraph_5utils_4read_7DataSet_14resetPosAndNegValid(((struct __pyx_obj_6kgraph_5utils_4read_DataSet *)__pyx_v_self), __pyx_v_flag);
 
@@ -10072,358 +10096,358 @@
   PyObject *__pyx_t_7 = NULL;
   __Pyx_memviewslice __pyx_t_8 = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("resetPosAndNegValid", 0);
 
-  /* "kgraph/utils/read.pyx":609
+  /* "kgraph/utils/read.pyx":621
  * 
  *     def resetPosAndNegValid(self, flag=False):
  *         valid_array = self.getValid()             # <<<<<<<<<<<<<<
  * 
  *         if flag:
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_getValid); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 609, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_getValid); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 621, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 609, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 621, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_valid_array = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "kgraph/utils/read.pyx":611
+  /* "kgraph/utils/read.pyx":623
  *         valid_array = self.getValid()
  * 
  *         if flag:             # <<<<<<<<<<<<<<
  *             idx = range(len(valid_array) // 2)
  *             pos_idx = [2 * x for x in idx]
  */
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_flag); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 611, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_flag); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 623, __pyx_L1_error)
   if (__pyx_t_4) {
 
-    /* "kgraph/utils/read.pyx":612
+    /* "kgraph/utils/read.pyx":624
  * 
  *         if flag:
  *             idx = range(len(valid_array) // 2)             # <<<<<<<<<<<<<<
  *             pos_idx = [2 * x for x in idx]
  *             neg_idx = [2 * x + 1 for x in idx]
  */
-    __pyx_t_5 = PyObject_Length(__pyx_v_valid_array); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 612, __pyx_L1_error)
-    __pyx_t_1 = PyInt_FromSsize_t(__Pyx_div_Py_ssize_t(__pyx_t_5, 2)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 612, __pyx_L1_error)
+    __pyx_t_5 = PyObject_Length(__pyx_v_valid_array); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 624, __pyx_L1_error)
+    __pyx_t_1 = PyInt_FromSsize_t(__Pyx_div_Py_ssize_t(__pyx_t_5, 2)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 624, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 612, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 624, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_v_idx = __pyx_t_2;
     __pyx_t_2 = 0;
 
-    /* "kgraph/utils/read.pyx":613
+    /* "kgraph/utils/read.pyx":625
  *         if flag:
  *             idx = range(len(valid_array) // 2)
  *             pos_idx = [2 * x for x in idx]             # <<<<<<<<<<<<<<
  *             neg_idx = [2 * x + 1 for x in idx]
  *             pos_valid_array = valid_array[pos_idx, :]
  */
     { /* enter inner scope */
-      __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 613, __pyx_L6_error)
+      __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 625, __pyx_L6_error)
       __Pyx_GOTREF(__pyx_t_2);
       if (likely(PyList_CheckExact(__pyx_v_idx)) || PyTuple_CheckExact(__pyx_v_idx)) {
         __pyx_t_1 = __pyx_v_idx; __Pyx_INCREF(__pyx_t_1); __pyx_t_5 = 0;
         __pyx_t_6 = NULL;
       } else {
-        __pyx_t_5 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_idx); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 613, __pyx_L6_error)
+        __pyx_t_5 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_idx); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 625, __pyx_L6_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_6 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 613, __pyx_L6_error)
+        __pyx_t_6 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 625, __pyx_L6_error)
       }
       for (;;) {
         if (likely(!__pyx_t_6)) {
           if (likely(PyList_CheckExact(__pyx_t_1))) {
             if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_1)) break;
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_3 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_3); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 613, __pyx_L6_error)
+            __pyx_t_3 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_3); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 625, __pyx_L6_error)
             #else
-            __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 613, __pyx_L6_error)
+            __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 625, __pyx_L6_error)
             __Pyx_GOTREF(__pyx_t_3);
             #endif
           } else {
             if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_3); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 613, __pyx_L6_error)
+            __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_3); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 625, __pyx_L6_error)
             #else
-            __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 613, __pyx_L6_error)
+            __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 625, __pyx_L6_error)
             __Pyx_GOTREF(__pyx_t_3);
             #endif
           }
         } else {
           __pyx_t_3 = __pyx_t_6(__pyx_t_1);
           if (unlikely(!__pyx_t_3)) {
             PyObject* exc_type = PyErr_Occurred();
             if (exc_type) {
               if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-              else __PYX_ERR(0, 613, __pyx_L6_error)
+              else __PYX_ERR(0, 625, __pyx_L6_error)
             }
             break;
           }
           __Pyx_GOTREF(__pyx_t_3);
         }
         __Pyx_XDECREF_SET(__pyx_8genexpr2__pyx_v_x, __pyx_t_3);
         __pyx_t_3 = 0;
-        __pyx_t_3 = PyNumber_Multiply(__pyx_int_2, __pyx_8genexpr2__pyx_v_x); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 613, __pyx_L6_error)
+        __pyx_t_3 = PyNumber_Multiply(__pyx_int_2, __pyx_8genexpr2__pyx_v_x); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 625, __pyx_L6_error)
         __Pyx_GOTREF(__pyx_t_3);
-        if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_3))) __PYX_ERR(0, 613, __pyx_L6_error)
+        if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_3))) __PYX_ERR(0, 625, __pyx_L6_error)
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       }
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_x); __pyx_8genexpr2__pyx_v_x = 0;
       goto __pyx_L9_exit_scope;
       __pyx_L6_error:;
       __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_x); __pyx_8genexpr2__pyx_v_x = 0;
       goto __pyx_L1_error;
       __pyx_L9_exit_scope:;
     } /* exit inner scope */
     __pyx_v_pos_idx = ((PyObject*)__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "kgraph/utils/read.pyx":614
+    /* "kgraph/utils/read.pyx":626
  *             idx = range(len(valid_array) // 2)
  *             pos_idx = [2 * x for x in idx]
  *             neg_idx = [2 * x + 1 for x in idx]             # <<<<<<<<<<<<<<
  *             pos_valid_array = valid_array[pos_idx, :]
  *             neg_valid_array = valid_array[neg_idx, :]
  */
     { /* enter inner scope */
-      __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 614, __pyx_L12_error)
+      __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 626, __pyx_L12_error)
       __Pyx_GOTREF(__pyx_t_2);
       if (likely(PyList_CheckExact(__pyx_v_idx)) || PyTuple_CheckExact(__pyx_v_idx)) {
         __pyx_t_1 = __pyx_v_idx; __Pyx_INCREF(__pyx_t_1); __pyx_t_5 = 0;
         __pyx_t_6 = NULL;
       } else {
-        __pyx_t_5 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_idx); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 614, __pyx_L12_error)
+        __pyx_t_5 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_idx); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 626, __pyx_L12_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_6 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 614, __pyx_L12_error)
+        __pyx_t_6 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 626, __pyx_L12_error)
       }
       for (;;) {
         if (likely(!__pyx_t_6)) {
           if (likely(PyList_CheckExact(__pyx_t_1))) {
             if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_1)) break;
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_3 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_3); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 614, __pyx_L12_error)
+            __pyx_t_3 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_3); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 626, __pyx_L12_error)
             #else
-            __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 614, __pyx_L12_error)
+            __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 626, __pyx_L12_error)
             __Pyx_GOTREF(__pyx_t_3);
             #endif
           } else {
             if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_3); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 614, __pyx_L12_error)
+            __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_3); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 626, __pyx_L12_error)
             #else
-            __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 614, __pyx_L12_error)
+            __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 626, __pyx_L12_error)
             __Pyx_GOTREF(__pyx_t_3);
             #endif
           }
         } else {
           __pyx_t_3 = __pyx_t_6(__pyx_t_1);
           if (unlikely(!__pyx_t_3)) {
             PyObject* exc_type = PyErr_Occurred();
             if (exc_type) {
               if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-              else __PYX_ERR(0, 614, __pyx_L12_error)
+              else __PYX_ERR(0, 626, __pyx_L12_error)
             }
             break;
           }
           __Pyx_GOTREF(__pyx_t_3);
         }
         __Pyx_XDECREF_SET(__pyx_8genexpr3__pyx_v_x, __pyx_t_3);
         __pyx_t_3 = 0;
-        __pyx_t_3 = PyNumber_Multiply(__pyx_int_2, __pyx_8genexpr3__pyx_v_x); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 614, __pyx_L12_error)
+        __pyx_t_3 = PyNumber_Multiply(__pyx_int_2, __pyx_8genexpr3__pyx_v_x); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 626, __pyx_L12_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_t_3, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 614, __pyx_L12_error)
+        __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_t_3, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 626, __pyx_L12_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_7))) __PYX_ERR(0, 614, __pyx_L12_error)
+        if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_7))) __PYX_ERR(0, 626, __pyx_L12_error)
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       }
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_x); __pyx_8genexpr3__pyx_v_x = 0;
       goto __pyx_L15_exit_scope;
       __pyx_L12_error:;
       __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_x); __pyx_8genexpr3__pyx_v_x = 0;
       goto __pyx_L1_error;
       __pyx_L15_exit_scope:;
     } /* exit inner scope */
     __pyx_v_neg_idx = ((PyObject*)__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "kgraph/utils/read.pyx":615
+    /* "kgraph/utils/read.pyx":627
  *             pos_idx = [2 * x for x in idx]
  *             neg_idx = [2 * x + 1 for x in idx]
  *             pos_valid_array = valid_array[pos_idx, :]             # <<<<<<<<<<<<<<
  *             neg_valid_array = valid_array[neg_idx, :]
  *             putValidInCache_c(&(self.valid_pos_data_ptr), pos_valid_array, self.num_ent, self.num_rel, self.tmp_memory_pool)
  */
-    __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 615, __pyx_L1_error)
+    __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 627, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_INCREF(__pyx_v_pos_idx);
     __Pyx_GIVEREF(__pyx_v_pos_idx);
     PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_pos_idx);
     __Pyx_INCREF(__pyx_slice_);
     __Pyx_GIVEREF(__pyx_slice_);
     PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_slice_);
-    __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_valid_array, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 615, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_valid_array, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 627, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_v_pos_valid_array = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "kgraph/utils/read.pyx":616
+    /* "kgraph/utils/read.pyx":628
  *             neg_idx = [2 * x + 1 for x in idx]
  *             pos_valid_array = valid_array[pos_idx, :]
  *             neg_valid_array = valid_array[neg_idx, :]             # <<<<<<<<<<<<<<
  *             putValidInCache_c(&(self.valid_pos_data_ptr), pos_valid_array, self.num_ent, self.num_rel, self.tmp_memory_pool)
  *             putValidInCache_c(&(self.valid_neg_data_ptr), neg_valid_array, self.num_ent, self.num_rel, self.tmp_memory_pool)
  */
-    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 616, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 628, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_v_neg_idx);
     __Pyx_GIVEREF(__pyx_v_neg_idx);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_neg_idx);
     __Pyx_INCREF(__pyx_slice_);
     __Pyx_GIVEREF(__pyx_slice_);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_slice_);
-    __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_v_valid_array, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 616, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_v_valid_array, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 628, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_v_neg_valid_array = __pyx_t_2;
     __pyx_t_2 = 0;
 
-    /* "kgraph/utils/read.pyx":617
+    /* "kgraph/utils/read.pyx":629
  *             pos_valid_array = valid_array[pos_idx, :]
  *             neg_valid_array = valid_array[neg_idx, :]
  *             putValidInCache_c(&(self.valid_pos_data_ptr), pos_valid_array, self.num_ent, self.num_rel, self.tmp_memory_pool)             # <<<<<<<<<<<<<<
  *             putValidInCache_c(&(self.valid_neg_data_ptr), neg_valid_array, self.num_ent, self.num_rel, self.tmp_memory_pool)
  *             putValidInCache_c(&(self.valid_data_ptr), pos_valid_array, self.num_ent, self.num_rel, self.tmp_memory_pool)
  */
-    __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int(__pyx_v_pos_valid_array, PyBUF_WRITABLE); if (unlikely(!__pyx_t_8.memview)) __PYX_ERR(0, 617, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int(__pyx_v_pos_valid_array, PyBUF_WRITABLE); if (unlikely(!__pyx_t_8.memview)) __PYX_ERR(0, 629, __pyx_L1_error)
     __pyx_t_2 = ((PyObject *)__pyx_v_self->tmp_memory_pool);
     __Pyx_INCREF(__pyx_t_2);
     __pyx_f_6kgraph_5utils_4read_putValidInCache_c((&__pyx_v_self->valid_pos_data_ptr), __pyx_t_8, __pyx_v_self->num_ent, __pyx_v_self->num_rel, ((struct __pyx_obj_6kgraph_5utils_6memory_MemoryPool *)__pyx_t_2));
     __PYX_XDEC_MEMVIEW(&__pyx_t_8, 1);
     __pyx_t_8.memview = NULL;
     __pyx_t_8.data = NULL;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "kgraph/utils/read.pyx":618
+    /* "kgraph/utils/read.pyx":630
  *             neg_valid_array = valid_array[neg_idx, :]
  *             putValidInCache_c(&(self.valid_pos_data_ptr), pos_valid_array, self.num_ent, self.num_rel, self.tmp_memory_pool)
  *             putValidInCache_c(&(self.valid_neg_data_ptr), neg_valid_array, self.num_ent, self.num_rel, self.tmp_memory_pool)             # <<<<<<<<<<<<<<
  *             putValidInCache_c(&(self.valid_data_ptr), pos_valid_array, self.num_ent, self.num_rel, self.tmp_memory_pool)
  *             self.triple_generate_negative_for_classification = 1
  */
-    __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int(__pyx_v_neg_valid_array, PyBUF_WRITABLE); if (unlikely(!__pyx_t_8.memview)) __PYX_ERR(0, 618, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int(__pyx_v_neg_valid_array, PyBUF_WRITABLE); if (unlikely(!__pyx_t_8.memview)) __PYX_ERR(0, 630, __pyx_L1_error)
     __pyx_t_2 = ((PyObject *)__pyx_v_self->tmp_memory_pool);
     __Pyx_INCREF(__pyx_t_2);
     __pyx_f_6kgraph_5utils_4read_putValidInCache_c((&__pyx_v_self->valid_neg_data_ptr), __pyx_t_8, __pyx_v_self->num_ent, __pyx_v_self->num_rel, ((struct __pyx_obj_6kgraph_5utils_6memory_MemoryPool *)__pyx_t_2));
     __PYX_XDEC_MEMVIEW(&__pyx_t_8, 1);
     __pyx_t_8.memview = NULL;
     __pyx_t_8.data = NULL;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "kgraph/utils/read.pyx":619
+    /* "kgraph/utils/read.pyx":631
  *             putValidInCache_c(&(self.valid_pos_data_ptr), pos_valid_array, self.num_ent, self.num_rel, self.tmp_memory_pool)
  *             putValidInCache_c(&(self.valid_neg_data_ptr), neg_valid_array, self.num_ent, self.num_rel, self.tmp_memory_pool)
  *             putValidInCache_c(&(self.valid_data_ptr), pos_valid_array, self.num_ent, self.num_rel, self.tmp_memory_pool)             # <<<<<<<<<<<<<<
  *             self.triple_generate_negative_for_classification = 1
  *         else:
  */
-    __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int(__pyx_v_pos_valid_array, PyBUF_WRITABLE); if (unlikely(!__pyx_t_8.memview)) __PYX_ERR(0, 619, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int(__pyx_v_pos_valid_array, PyBUF_WRITABLE); if (unlikely(!__pyx_t_8.memview)) __PYX_ERR(0, 631, __pyx_L1_error)
     __pyx_t_2 = ((PyObject *)__pyx_v_self->tmp_memory_pool);
     __Pyx_INCREF(__pyx_t_2);
     __pyx_f_6kgraph_5utils_4read_putValidInCache_c((&__pyx_v_self->valid_data_ptr), __pyx_t_8, __pyx_v_self->num_ent, __pyx_v_self->num_rel, ((struct __pyx_obj_6kgraph_5utils_6memory_MemoryPool *)__pyx_t_2));
     __PYX_XDEC_MEMVIEW(&__pyx_t_8, 1);
     __pyx_t_8.memview = NULL;
     __pyx_t_8.data = NULL;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "kgraph/utils/read.pyx":620
+    /* "kgraph/utils/read.pyx":632
  *             putValidInCache_c(&(self.valid_neg_data_ptr), neg_valid_array, self.num_ent, self.num_rel, self.tmp_memory_pool)
  *             putValidInCache_c(&(self.valid_data_ptr), pos_valid_array, self.num_ent, self.num_rel, self.tmp_memory_pool)
  *             self.triple_generate_negative_for_classification = 1             # <<<<<<<<<<<<<<
  *         else:
  *             putValidInCache_c(&(self.valid_pos_data_ptr), valid_array, self.num_ent, self.num_rel, self.tmp_memory_pool)
  */
     __pyx_v_self->triple_generate_negative_for_classification = 1;
 
-    /* "kgraph/utils/read.pyx":611
+    /* "kgraph/utils/read.pyx":623
  *         valid_array = self.getValid()
  * 
  *         if flag:             # <<<<<<<<<<<<<<
  *             idx = range(len(valid_array) // 2)
  *             pos_idx = [2 * x for x in idx]
  */
     goto __pyx_L3;
   }
 
-  /* "kgraph/utils/read.pyx":622
+  /* "kgraph/utils/read.pyx":634
  *             self.triple_generate_negative_for_classification = 1
  *         else:
  *             putValidInCache_c(&(self.valid_pos_data_ptr), valid_array, self.num_ent, self.num_rel, self.tmp_memory_pool)             # <<<<<<<<<<<<<<
  *             putValidInCache_c(&(self.valid_neg_data_ptr), valid_array, self.num_ent, self.num_rel, self.tmp_memory_pool)
  *             self.triple_generate_negative_for_classification = 0
  */
   /*else*/ {
-    __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int(__pyx_v_valid_array, PyBUF_WRITABLE); if (unlikely(!__pyx_t_8.memview)) __PYX_ERR(0, 622, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int(__pyx_v_valid_array, PyBUF_WRITABLE); if (unlikely(!__pyx_t_8.memview)) __PYX_ERR(0, 634, __pyx_L1_error)
     __pyx_t_2 = ((PyObject *)__pyx_v_self->tmp_memory_pool);
     __Pyx_INCREF(__pyx_t_2);
     __pyx_f_6kgraph_5utils_4read_putValidInCache_c((&__pyx_v_self->valid_pos_data_ptr), __pyx_t_8, __pyx_v_self->num_ent, __pyx_v_self->num_rel, ((struct __pyx_obj_6kgraph_5utils_6memory_MemoryPool *)__pyx_t_2));
     __PYX_XDEC_MEMVIEW(&__pyx_t_8, 1);
     __pyx_t_8.memview = NULL;
     __pyx_t_8.data = NULL;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "kgraph/utils/read.pyx":623
+    /* "kgraph/utils/read.pyx":635
  *         else:
  *             putValidInCache_c(&(self.valid_pos_data_ptr), valid_array, self.num_ent, self.num_rel, self.tmp_memory_pool)
  *             putValidInCache_c(&(self.valid_neg_data_ptr), valid_array, self.num_ent, self.num_rel, self.tmp_memory_pool)             # <<<<<<<<<<<<<<
  *             self.triple_generate_negative_for_classification = 0
  * 
  */
-    __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int(__pyx_v_valid_array, PyBUF_WRITABLE); if (unlikely(!__pyx_t_8.memview)) __PYX_ERR(0, 623, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int(__pyx_v_valid_array, PyBUF_WRITABLE); if (unlikely(!__pyx_t_8.memview)) __PYX_ERR(0, 635, __pyx_L1_error)
     __pyx_t_2 = ((PyObject *)__pyx_v_self->tmp_memory_pool);
     __Pyx_INCREF(__pyx_t_2);
     __pyx_f_6kgraph_5utils_4read_putValidInCache_c((&__pyx_v_self->valid_neg_data_ptr), __pyx_t_8, __pyx_v_self->num_ent, __pyx_v_self->num_rel, ((struct __pyx_obj_6kgraph_5utils_6memory_MemoryPool *)__pyx_t_2));
     __PYX_XDEC_MEMVIEW(&__pyx_t_8, 1);
     __pyx_t_8.memview = NULL;
     __pyx_t_8.data = NULL;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "kgraph/utils/read.pyx":624
+    /* "kgraph/utils/read.pyx":636
  *             putValidInCache_c(&(self.valid_pos_data_ptr), valid_array, self.num_ent, self.num_rel, self.tmp_memory_pool)
  *             putValidInCache_c(&(self.valid_neg_data_ptr), valid_array, self.num_ent, self.num_rel, self.tmp_memory_pool)
  *             self.triple_generate_negative_for_classification = 0             # <<<<<<<<<<<<<<
  * 
  *     def initConstraint(self):
  */
     __pyx_v_self->triple_generate_negative_for_classification = 0;
   }
   __pyx_L3:;
 
-  /* "kgraph/utils/read.pyx":608
+  /* "kgraph/utils/read.pyx":620
  *             self.triple_generate_negative_for_classification = 0
  * 
  *     def resetPosAndNegValid(self, flag=False):             # <<<<<<<<<<<<<<
  *         valid_array = self.getValid()
  * 
  */
 
@@ -10448,15 +10472,15 @@
   __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_x);
   __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_x);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kgraph/utils/read.pyx":626
+/* "kgraph/utils/read.pyx":638
  *             self.triple_generate_negative_for_classification = 0
  * 
  *     def initConstraint(self):             # <<<<<<<<<<<<<<
  *         global type_constrain
  *         # global all_triples
  */
 
@@ -10475,42 +10499,42 @@
 
 static PyObject *__pyx_pf_6kgraph_5utils_4read_7DataSet_16initConstraint(struct __pyx_obj_6kgraph_5utils_4read_DataSet *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("initConstraint", 0);
 
-  /* "kgraph/utils/read.pyx":629
+  /* "kgraph/utils/read.pyx":641
  *         global type_constrain
  *         # global all_triples
  *         get_constrain(&type_constrain, &(self.all_triples_ptr), self.num_rel, self.tmp_memory_pool)             # <<<<<<<<<<<<<<
  * 
  *     def resetAllInCache(self, int[:, ::1] train_data, int[:, ::1] valid_data, int[:, ::1] test_data):
  */
   __pyx_t_1 = ((PyObject *)__pyx_v_self->tmp_memory_pool);
   __Pyx_INCREF(__pyx_t_1);
   __pyx_f_6kgraph_5utils_4read_get_constrain((&__pyx_v_6kgraph_5utils_4read_type_constrain), (&__pyx_v_self->all_triples_ptr), __pyx_v_self->num_rel, ((struct __pyx_obj_6kgraph_5utils_6memory_MemoryPool *)__pyx_t_1));
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "kgraph/utils/read.pyx":626
+  /* "kgraph/utils/read.pyx":638
  *             self.triple_generate_negative_for_classification = 0
  * 
  *     def initConstraint(self):             # <<<<<<<<<<<<<<
  *         global type_constrain
  *         # global all_triples
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kgraph/utils/read.pyx":631
+/* "kgraph/utils/read.pyx":643
  *         get_constrain(&type_constrain, &(self.all_triples_ptr), self.num_rel, self.tmp_memory_pool)
  * 
  *     def resetAllInCache(self, int[:, ::1] train_data, int[:, ::1] valid_data, int[:, ::1] test_data):             # <<<<<<<<<<<<<<
  * 
  *         self.train = train_data
  */
 
@@ -10547,40 +10571,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_train_data)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_valid_data)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("resetAllInCache", 1, 3, 3, 1); __PYX_ERR(0, 631, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("resetAllInCache", 1, 3, 3, 1); __PYX_ERR(0, 643, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_test_data)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("resetAllInCache", 1, 3, 3, 2); __PYX_ERR(0, 631, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("resetAllInCache", 1, 3, 3, 2); __PYX_ERR(0, 643, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "resetAllInCache") < 0)) __PYX_ERR(0, 631, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "resetAllInCache") < 0)) __PYX_ERR(0, 643, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
-    __pyx_v_train_data = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_train_data.memview)) __PYX_ERR(0, 631, __pyx_L3_error)
-    __pyx_v_valid_data = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_valid_data.memview)) __PYX_ERR(0, 631, __pyx_L3_error)
-    __pyx_v_test_data = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_test_data.memview)) __PYX_ERR(0, 631, __pyx_L3_error)
+    __pyx_v_train_data = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_train_data.memview)) __PYX_ERR(0, 643, __pyx_L3_error)
+    __pyx_v_valid_data = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_valid_data.memview)) __PYX_ERR(0, 643, __pyx_L3_error)
+    __pyx_v_test_data = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_test_data.memview)) __PYX_ERR(0, 643, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("resetAllInCache", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 631, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("resetAllInCache", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 643, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("kgraph.utils.read.DataSet.resetAllInCache", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6kgraph_5utils_4read_7DataSet_18resetAllInCache(((struct __pyx_obj_6kgraph_5utils_4read_DataSet *)__pyx_v_self), __pyx_v_train_data, __pyx_v_valid_data, __pyx_v_test_data);
 
@@ -10596,77 +10620,77 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("resetAllInCache", 0);
 
-  /* "kgraph/utils/read.pyx":633
+  /* "kgraph/utils/read.pyx":645
  *     def resetAllInCache(self, int[:, ::1] train_data, int[:, ::1] valid_data, int[:, ::1] test_data):
  * 
  *         self.train = train_data             # <<<<<<<<<<<<<<
  *         self.valid = valid_data
  *         self.test = test_data
  */
-  __pyx_t_1 = __pyx_memoryview_fromslice(__pyx_v_train_data, 2, (PyObject *(*)(char *)) __pyx_memview_get_int, (int (*)(char *, PyObject *)) __pyx_memview_set_int, 0);; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 633, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_fromslice(__pyx_v_train_data, 2, (PyObject *(*)(char *)) __pyx_memview_get_int, (int (*)(char *, PyObject *)) __pyx_memview_set_int, 0);; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 645, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_PyObject_SetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_train, __pyx_t_1) < 0) __PYX_ERR(0, 633, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_train, __pyx_t_1) < 0) __PYX_ERR(0, 645, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "kgraph/utils/read.pyx":634
+  /* "kgraph/utils/read.pyx":646
  * 
  *         self.train = train_data
  *         self.valid = valid_data             # <<<<<<<<<<<<<<
  *         self.test = test_data
  *         self.update()
  */
-  __pyx_t_1 = __pyx_memoryview_fromslice(__pyx_v_valid_data, 2, (PyObject *(*)(char *)) __pyx_memview_get_int, (int (*)(char *, PyObject *)) __pyx_memview_set_int, 0);; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 634, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_fromslice(__pyx_v_valid_data, 2, (PyObject *(*)(char *)) __pyx_memview_get_int, (int (*)(char *, PyObject *)) __pyx_memview_set_int, 0);; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 646, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_PyObject_SetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_valid, __pyx_t_1) < 0) __PYX_ERR(0, 634, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_valid, __pyx_t_1) < 0) __PYX_ERR(0, 646, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "kgraph/utils/read.pyx":635
+  /* "kgraph/utils/read.pyx":647
  *         self.train = train_data
  *         self.valid = valid_data
  *         self.test = test_data             # <<<<<<<<<<<<<<
  *         self.update()
  * 
  */
-  __pyx_t_1 = __pyx_memoryview_fromslice(__pyx_v_test_data, 2, (PyObject *(*)(char *)) __pyx_memview_get_int, (int (*)(char *, PyObject *)) __pyx_memview_set_int, 0);; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 635, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_fromslice(__pyx_v_test_data, 2, (PyObject *(*)(char *)) __pyx_memview_get_int, (int (*)(char *, PyObject *)) __pyx_memview_set_int, 0);; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 647, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_PyObject_SetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 635, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 647, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "kgraph/utils/read.pyx":636
+  /* "kgraph/utils/read.pyx":648
  *         self.valid = valid_data
  *         self.test = test_data
  *         self.update()             # <<<<<<<<<<<<<<
  * 
  *     def update(self):
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_update); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 636, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_update); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 648, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 636, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 648, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "kgraph/utils/read.pyx":631
+  /* "kgraph/utils/read.pyx":643
  *         get_constrain(&type_constrain, &(self.all_triples_ptr), self.num_rel, self.tmp_memory_pool)
  * 
  *     def resetAllInCache(self, int[:, ::1] train_data, int[:, ::1] valid_data, int[:, ::1] test_data):             # <<<<<<<<<<<<<<
  * 
  *         self.train = train_data
  */
 
@@ -10684,15 +10708,15 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_valid_data, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_test_data, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kgraph/utils/read.pyx":638
+/* "kgraph/utils/read.pyx":650
  *         self.update()
  * 
  *     def update(self):             # <<<<<<<<<<<<<<
  *         putAllInCache_c(&(self.all_triples_ptr),
  *                         getDataFromCache_c(&(self.train_data_ptr)),
  */
 
@@ -10717,61 +10741,61 @@
   __Pyx_memviewslice __pyx_t_3 = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_t_4 = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("update", 0);
 
-  /* "kgraph/utils/read.pyx":640
+  /* "kgraph/utils/read.pyx":652
  *     def update(self):
  *         putAllInCache_c(&(self.all_triples_ptr),
  *                         getDataFromCache_c(&(self.train_data_ptr)),             # <<<<<<<<<<<<<<
  *                         getDataFromCache_c(&(self.valid_data_ptr)),
  *                         getDataFromCache_c(&(self.test_data_ptr)),
  */
-  __pyx_t_1 = ((PyObject *)__pyx_f_6kgraph_5utils_4read_getDataFromCache_c((&__pyx_v_self->train_data_ptr))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 640, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__pyx_f_6kgraph_5utils_4read_getDataFromCache_c((&__pyx_v_self->train_data_ptr))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 652, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 640, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 652, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "kgraph/utils/read.pyx":641
+  /* "kgraph/utils/read.pyx":653
  *         putAllInCache_c(&(self.all_triples_ptr),
  *                         getDataFromCache_c(&(self.train_data_ptr)),
  *                         getDataFromCache_c(&(self.valid_data_ptr)),             # <<<<<<<<<<<<<<
  *                         getDataFromCache_c(&(self.test_data_ptr)),
  *                         self.num_ent, self.num_rel, self.tmp_memory_pool)
  */
-  __pyx_t_1 = ((PyObject *)__pyx_f_6kgraph_5utils_4read_getDataFromCache_c((&__pyx_v_self->valid_data_ptr))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 641, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__pyx_f_6kgraph_5utils_4read_getDataFromCache_c((&__pyx_v_self->valid_data_ptr))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 653, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_3.memview)) __PYX_ERR(0, 641, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_3.memview)) __PYX_ERR(0, 653, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "kgraph/utils/read.pyx":642
+  /* "kgraph/utils/read.pyx":654
  *                         getDataFromCache_c(&(self.train_data_ptr)),
  *                         getDataFromCache_c(&(self.valid_data_ptr)),
  *                         getDataFromCache_c(&(self.test_data_ptr)),             # <<<<<<<<<<<<<<
  *                         self.num_ent, self.num_rel, self.tmp_memory_pool)
  * 
  */
-  __pyx_t_1 = ((PyObject *)__pyx_f_6kgraph_5utils_4read_getDataFromCache_c((&__pyx_v_self->test_data_ptr))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 642, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__pyx_f_6kgraph_5utils_4read_getDataFromCache_c((&__pyx_v_self->test_data_ptr))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 654, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_4.memview)) __PYX_ERR(0, 642, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_4.memview)) __PYX_ERR(0, 654, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "kgraph/utils/read.pyx":643
+  /* "kgraph/utils/read.pyx":655
  *                         getDataFromCache_c(&(self.valid_data_ptr)),
  *                         getDataFromCache_c(&(self.test_data_ptr)),
  *                         self.num_ent, self.num_rel, self.tmp_memory_pool)             # <<<<<<<<<<<<<<
  * 
  *     property trainArray:
  */
   __pyx_t_1 = ((PyObject *)__pyx_v_self->tmp_memory_pool);
   __Pyx_INCREF(__pyx_t_1);
 
-  /* "kgraph/utils/read.pyx":639
+  /* "kgraph/utils/read.pyx":651
  * 
  *     def update(self):
  *         putAllInCache_c(&(self.all_triples_ptr),             # <<<<<<<<<<<<<<
  *                         getDataFromCache_c(&(self.train_data_ptr)),
  *                         getDataFromCache_c(&(self.valid_data_ptr)),
  */
   __pyx_f_6kgraph_5utils_4read_putAllInCache_c((&__pyx_v_self->all_triples_ptr), __pyx_t_2, __pyx_t_3, __pyx_t_4, __pyx_v_self->num_ent, __pyx_v_self->num_rel, ((struct __pyx_obj_6kgraph_5utils_6memory_MemoryPool *)__pyx_t_1));
@@ -10782,15 +10806,15 @@
   __pyx_t_3.memview = NULL;
   __pyx_t_3.data = NULL;
   __PYX_XDEC_MEMVIEW(&__pyx_t_4, 1);
   __pyx_t_4.memview = NULL;
   __pyx_t_4.data = NULL;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "kgraph/utils/read.pyx":638
+  /* "kgraph/utils/read.pyx":650
  *         self.update()
  * 
  *     def update(self):             # <<<<<<<<<<<<<<
  *         putAllInCache_c(&(self.all_triples_ptr),
  *                         getDataFromCache_c(&(self.train_data_ptr)),
  */
 
@@ -10806,15 +10830,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kgraph/utils/read.pyx":646
+/* "kgraph/utils/read.pyx":658
  * 
  *     property trainArray:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return getDataFromCache_c(&(self.train_data_ptr))
  * 
  */
 
@@ -10836,29 +10860,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "kgraph/utils/read.pyx":647
+  /* "kgraph/utils/read.pyx":659
  *     property trainArray:
  *         def __get__(self):
  *             return getDataFromCache_c(&(self.train_data_ptr))             # <<<<<<<<<<<<<<
  * 
  *         def __set__(self, int[:, ::1] value):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = ((PyObject *)__pyx_f_6kgraph_5utils_4read_getDataFromCache_c((&__pyx_v_self->train_data_ptr))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 647, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__pyx_f_6kgraph_5utils_4read_getDataFromCache_c((&__pyx_v_self->train_data_ptr))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 659, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "kgraph/utils/read.pyx":646
+  /* "kgraph/utils/read.pyx":658
  * 
  *     property trainArray:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return getDataFromCache_c(&(self.train_data_ptr))
  * 
  */
 
@@ -10869,15 +10893,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kgraph/utils/read.pyx":649
+/* "kgraph/utils/read.pyx":661
  *             return getDataFromCache_c(&(self.train_data_ptr))
  * 
  *         def __set__(self, int[:, ::1] value):             # <<<<<<<<<<<<<<
  *             putTrainInCache_c(&(self.train_data_ptr), value, self.num_ent, self.num_rel, self.tmp_memory_pool)
  *             self.__calculate_train_data_size()
  */
 
@@ -10888,15 +10912,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
   assert(__pyx_arg_value); {
-    __pyx_v_value = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int(__pyx_arg_value, PyBUF_WRITABLE); if (unlikely(!__pyx_v_value.memview)) __PYX_ERR(0, 649, __pyx_L3_error)
+    __pyx_v_value = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int(__pyx_arg_value, PyBUF_WRITABLE); if (unlikely(!__pyx_v_value.memview)) __PYX_ERR(0, 661, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("kgraph.utils.read.DataSet.trainArray.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
@@ -10914,53 +10938,53 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
 
-  /* "kgraph/utils/read.pyx":650
+  /* "kgraph/utils/read.pyx":662
  * 
  *         def __set__(self, int[:, ::1] value):
  *             putTrainInCache_c(&(self.train_data_ptr), value, self.num_ent, self.num_rel, self.tmp_memory_pool)             # <<<<<<<<<<<<<<
  *             self.__calculate_train_data_size()
  * 
  */
   __pyx_t_1 = ((PyObject *)__pyx_v_self->tmp_memory_pool);
   __Pyx_INCREF(__pyx_t_1);
   __pyx_f_6kgraph_5utils_4read_putTrainInCache_c((&__pyx_v_self->train_data_ptr), __pyx_v_value, __pyx_v_self->num_ent, __pyx_v_self->num_rel, ((struct __pyx_obj_6kgraph_5utils_6memory_MemoryPool *)__pyx_t_1));
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "kgraph/utils/read.pyx":651
+  /* "kgraph/utils/read.pyx":663
  *         def __set__(self, int[:, ::1] value):
  *             putTrainInCache_c(&(self.train_data_ptr), value, self.num_ent, self.num_rel, self.tmp_memory_pool)
  *             self.__calculate_train_data_size()             # <<<<<<<<<<<<<<
  * 
  *     property validArray:
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_calculate_train_data_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 651, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_calculate_train_data_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 663, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 651, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 663, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "kgraph/utils/read.pyx":649
+  /* "kgraph/utils/read.pyx":661
  *             return getDataFromCache_c(&(self.train_data_ptr))
  * 
  *         def __set__(self, int[:, ::1] value):             # <<<<<<<<<<<<<<
  *             putTrainInCache_c(&(self.train_data_ptr), value, self.num_ent, self.num_rel, self.tmp_memory_pool)
  *             self.__calculate_train_data_size()
  */
 
@@ -10975,15 +10999,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __PYX_XDEC_MEMVIEW(&__pyx_v_value, 1);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kgraph/utils/read.pyx":654
+/* "kgraph/utils/read.pyx":666
  * 
  *     property validArray:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return getDataFromCache_c(&(self.valid_data_ptr))
  * 
  */
 
@@ -11005,29 +11029,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "kgraph/utils/read.pyx":655
+  /* "kgraph/utils/read.pyx":667
  *     property validArray:
  *         def __get__(self):
  *             return getDataFromCache_c(&(self.valid_data_ptr))             # <<<<<<<<<<<<<<
  * 
  *         def __set__(self, int[:, ::1] value):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = ((PyObject *)__pyx_f_6kgraph_5utils_4read_getDataFromCache_c((&__pyx_v_self->valid_data_ptr))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 655, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__pyx_f_6kgraph_5utils_4read_getDataFromCache_c((&__pyx_v_self->valid_data_ptr))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 667, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "kgraph/utils/read.pyx":654
+  /* "kgraph/utils/read.pyx":666
  * 
  *     property validArray:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return getDataFromCache_c(&(self.valid_data_ptr))
  * 
  */
 
@@ -11038,15 +11062,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kgraph/utils/read.pyx":657
+/* "kgraph/utils/read.pyx":669
  *             return getDataFromCache_c(&(self.valid_data_ptr))
  * 
  *         def __set__(self, int[:, ::1] value):             # <<<<<<<<<<<<<<
  *             putValidInCache_c(&(self.valid_data_ptr), value, self.num_ent, self.num_rel, self.tmp_memory_pool)
  * 
  */
 
@@ -11057,15 +11081,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
   assert(__pyx_arg_value); {
-    __pyx_v_value = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int(__pyx_arg_value, PyBUF_WRITABLE); if (unlikely(!__pyx_v_value.memview)) __PYX_ERR(0, 657, __pyx_L3_error)
+    __pyx_v_value = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int(__pyx_arg_value, PyBUF_WRITABLE); if (unlikely(!__pyx_v_value.memview)) __PYX_ERR(0, 669, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("kgraph.utils.read.DataSet.validArray.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
@@ -11078,42 +11102,42 @@
 
 static int __pyx_pf_6kgraph_5utils_4read_7DataSet_10validArray_2__set__(struct __pyx_obj_6kgraph_5utils_4read_DataSet *__pyx_v_self, __Pyx_memviewslice __pyx_v_value) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("__set__", 0);
 
-  /* "kgraph/utils/read.pyx":658
+  /* "kgraph/utils/read.pyx":670
  * 
  *         def __set__(self, int[:, ::1] value):
  *             putValidInCache_c(&(self.valid_data_ptr), value, self.num_ent, self.num_rel, self.tmp_memory_pool)             # <<<<<<<<<<<<<<
  * 
  *     property testArray:
  */
   __pyx_t_1 = ((PyObject *)__pyx_v_self->tmp_memory_pool);
   __Pyx_INCREF(__pyx_t_1);
   __pyx_f_6kgraph_5utils_4read_putValidInCache_c((&__pyx_v_self->valid_data_ptr), __pyx_v_value, __pyx_v_self->num_ent, __pyx_v_self->num_rel, ((struct __pyx_obj_6kgraph_5utils_6memory_MemoryPool *)__pyx_t_1));
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "kgraph/utils/read.pyx":657
+  /* "kgraph/utils/read.pyx":669
  *             return getDataFromCache_c(&(self.valid_data_ptr))
  * 
  *         def __set__(self, int[:, ::1] value):             # <<<<<<<<<<<<<<
  *             putValidInCache_c(&(self.valid_data_ptr), value, self.num_ent, self.num_rel, self.tmp_memory_pool)
  * 
  */
 
   /* function exit code */
   __pyx_r = 0;
   __PYX_XDEC_MEMVIEW(&__pyx_v_value, 1);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kgraph/utils/read.pyx":661
+/* "kgraph/utils/read.pyx":673
  * 
  *     property testArray:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return getDataFromCache_c(&(self.test_data_ptr))
  * 
  */
 
@@ -11135,29 +11159,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "kgraph/utils/read.pyx":662
+  /* "kgraph/utils/read.pyx":674
  *     property testArray:
  *         def __get__(self):
  *             return getDataFromCache_c(&(self.test_data_ptr))             # <<<<<<<<<<<<<<
  * 
  *         def __set__(self, int[:, ::1] value):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = ((PyObject *)__pyx_f_6kgraph_5utils_4read_getDataFromCache_c((&__pyx_v_self->test_data_ptr))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 662, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__pyx_f_6kgraph_5utils_4read_getDataFromCache_c((&__pyx_v_self->test_data_ptr))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 674, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "kgraph/utils/read.pyx":661
+  /* "kgraph/utils/read.pyx":673
  * 
  *     property testArray:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return getDataFromCache_c(&(self.test_data_ptr))
  * 
  */
 
@@ -11168,15 +11192,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kgraph/utils/read.pyx":664
+/* "kgraph/utils/read.pyx":676
  *             return getDataFromCache_c(&(self.test_data_ptr))
  * 
  *         def __set__(self, int[:, ::1] value):             # <<<<<<<<<<<<<<
  *             putTestInCache_c(&(self.test_data_ptr), value, self.num_ent, self.num_rel, self.tmp_memory_pool)
  * 
  */
 
@@ -11187,15 +11211,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
   assert(__pyx_arg_value); {
-    __pyx_v_value = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int(__pyx_arg_value, PyBUF_WRITABLE); if (unlikely(!__pyx_v_value.memview)) __PYX_ERR(0, 664, __pyx_L3_error)
+    __pyx_v_value = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int(__pyx_arg_value, PyBUF_WRITABLE); if (unlikely(!__pyx_v_value.memview)) __PYX_ERR(0, 676, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("kgraph.utils.read.DataSet.testArray.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
@@ -11208,42 +11232,42 @@
 
 static int __pyx_pf_6kgraph_5utils_4read_7DataSet_9testArray_2__set__(struct __pyx_obj_6kgraph_5utils_4read_DataSet *__pyx_v_self, __Pyx_memviewslice __pyx_v_value) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("__set__", 0);
 
-  /* "kgraph/utils/read.pyx":665
+  /* "kgraph/utils/read.pyx":677
  * 
  *         def __set__(self, int[:, ::1] value):
  *             putTestInCache_c(&(self.test_data_ptr), value, self.num_ent, self.num_rel, self.tmp_memory_pool)             # <<<<<<<<<<<<<<
  * 
  *     property train:
  */
   __pyx_t_1 = ((PyObject *)__pyx_v_self->tmp_memory_pool);
   __Pyx_INCREF(__pyx_t_1);
   __pyx_f_6kgraph_5utils_4read_putTestInCache_c((&__pyx_v_self->test_data_ptr), __pyx_v_value, __pyx_v_self->num_ent, __pyx_v_self->num_rel, ((struct __pyx_obj_6kgraph_5utils_6memory_MemoryPool *)__pyx_t_1));
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "kgraph/utils/read.pyx":664
+  /* "kgraph/utils/read.pyx":676
  *             return getDataFromCache_c(&(self.test_data_ptr))
  * 
  *         def __set__(self, int[:, ::1] value):             # <<<<<<<<<<<<<<
  *             putTestInCache_c(&(self.test_data_ptr), value, self.num_ent, self.num_rel, self.tmp_memory_pool)
  * 
  */
 
   /* function exit code */
   __pyx_r = 0;
   __PYX_XDEC_MEMVIEW(&__pyx_v_value, 1);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kgraph/utils/read.pyx":668
+/* "kgraph/utils/read.pyx":680
  * 
  *     property train:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return self.trainArray
  * 
  */
 
@@ -11265,29 +11289,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "kgraph/utils/read.pyx":669
+  /* "kgraph/utils/read.pyx":681
  *     property train:
  *         def __get__(self):
  *             return self.trainArray             # <<<<<<<<<<<<<<
  * 
  *         def __set__(self, int[:, ::1] value):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_trainArray); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 669, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_trainArray); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 681, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "kgraph/utils/read.pyx":668
+  /* "kgraph/utils/read.pyx":680
  * 
  *     property train:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return self.trainArray
  * 
  */
 
@@ -11298,15 +11322,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kgraph/utils/read.pyx":671
+/* "kgraph/utils/read.pyx":683
  *             return self.trainArray
  * 
  *         def __set__(self, int[:, ::1] value):             # <<<<<<<<<<<<<<
  *             self.trainArray = value
  * 
  */
 
@@ -11317,15 +11341,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
   assert(__pyx_arg_value); {
-    __pyx_v_value = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int(__pyx_arg_value, PyBUF_WRITABLE); if (unlikely(!__pyx_v_value.memview)) __PYX_ERR(0, 671, __pyx_L3_error)
+    __pyx_v_value = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int(__pyx_arg_value, PyBUF_WRITABLE); if (unlikely(!__pyx_v_value.memview)) __PYX_ERR(0, 683, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("kgraph.utils.read.DataSet.train.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
@@ -11341,27 +11365,27 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
 
-  /* "kgraph/utils/read.pyx":672
+  /* "kgraph/utils/read.pyx":684
  * 
  *         def __set__(self, int[:, ::1] value):
  *             self.trainArray = value             # <<<<<<<<<<<<<<
  * 
  *     property valid:
  */
-  __pyx_t_1 = __pyx_memoryview_fromslice(__pyx_v_value, 2, (PyObject *(*)(char *)) __pyx_memview_get_int, (int (*)(char *, PyObject *)) __pyx_memview_set_int, 0);; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 672, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_fromslice(__pyx_v_value, 2, (PyObject *(*)(char *)) __pyx_memview_get_int, (int (*)(char *, PyObject *)) __pyx_memview_set_int, 0);; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 684, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_PyObject_SetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_trainArray, __pyx_t_1) < 0) __PYX_ERR(0, 672, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_trainArray, __pyx_t_1) < 0) __PYX_ERR(0, 684, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "kgraph/utils/read.pyx":671
+  /* "kgraph/utils/read.pyx":683
  *             return self.trainArray
  * 
  *         def __set__(self, int[:, ::1] value):             # <<<<<<<<<<<<<<
  *             self.trainArray = value
  * 
  */
 
@@ -11374,15 +11398,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __PYX_XDEC_MEMVIEW(&__pyx_v_value, 1);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kgraph/utils/read.pyx":675
+/* "kgraph/utils/read.pyx":687
  * 
  *     property valid:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return self.validArray
  * 
  */
 
@@ -11404,29 +11428,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "kgraph/utils/read.pyx":676
+  /* "kgraph/utils/read.pyx":688
  *     property valid:
  *         def __get__(self):
  *             return self.validArray             # <<<<<<<<<<<<<<
  * 
  *         def __set__(self, int[:, ::1] value):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_validArray); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 676, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_validArray); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 688, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "kgraph/utils/read.pyx":675
+  /* "kgraph/utils/read.pyx":687
  * 
  *     property valid:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return self.validArray
  * 
  */
 
@@ -11437,15 +11461,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kgraph/utils/read.pyx":678
+/* "kgraph/utils/read.pyx":690
  *             return self.validArray
  * 
  *         def __set__(self, int[:, ::1] value):             # <<<<<<<<<<<<<<
  *             self.validArray = value
  * 
  */
 
@@ -11456,15 +11480,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
   assert(__pyx_arg_value); {
-    __pyx_v_value = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int(__pyx_arg_value, PyBUF_WRITABLE); if (unlikely(!__pyx_v_value.memview)) __PYX_ERR(0, 678, __pyx_L3_error)
+    __pyx_v_value = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int(__pyx_arg_value, PyBUF_WRITABLE); if (unlikely(!__pyx_v_value.memview)) __PYX_ERR(0, 690, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("kgraph.utils.read.DataSet.valid.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
@@ -11480,27 +11504,27 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
 
-  /* "kgraph/utils/read.pyx":679
+  /* "kgraph/utils/read.pyx":691
  * 
  *         def __set__(self, int[:, ::1] value):
  *             self.validArray = value             # <<<<<<<<<<<<<<
  * 
  *     property test:
  */
-  __pyx_t_1 = __pyx_memoryview_fromslice(__pyx_v_value, 2, (PyObject *(*)(char *)) __pyx_memview_get_int, (int (*)(char *, PyObject *)) __pyx_memview_set_int, 0);; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 679, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_fromslice(__pyx_v_value, 2, (PyObject *(*)(char *)) __pyx_memview_get_int, (int (*)(char *, PyObject *)) __pyx_memview_set_int, 0);; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 691, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_PyObject_SetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_validArray, __pyx_t_1) < 0) __PYX_ERR(0, 679, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_validArray, __pyx_t_1) < 0) __PYX_ERR(0, 691, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "kgraph/utils/read.pyx":678
+  /* "kgraph/utils/read.pyx":690
  *             return self.validArray
  * 
  *         def __set__(self, int[:, ::1] value):             # <<<<<<<<<<<<<<
  *             self.validArray = value
  * 
  */
 
@@ -11513,15 +11537,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __PYX_XDEC_MEMVIEW(&__pyx_v_value, 1);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kgraph/utils/read.pyx":682
+/* "kgraph/utils/read.pyx":694
  * 
  *     property test:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return self.testArray
  * 
  */
 
@@ -11543,29 +11567,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "kgraph/utils/read.pyx":683
+  /* "kgraph/utils/read.pyx":695
  *     property test:
  *         def __get__(self):
  *             return self.testArray             # <<<<<<<<<<<<<<
  * 
  *         def __set__(self, int[:, ::1] value):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_testArray); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 683, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_testArray); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 695, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "kgraph/utils/read.pyx":682
+  /* "kgraph/utils/read.pyx":694
  * 
  *     property test:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return self.testArray
  * 
  */
 
@@ -11576,15 +11600,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kgraph/utils/read.pyx":685
+/* "kgraph/utils/read.pyx":697
  *             return self.testArray
  * 
  *         def __set__(self, int[:, ::1] value):             # <<<<<<<<<<<<<<
  *             self.testArray = value
  * 
  */
 
@@ -11595,15 +11619,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
   assert(__pyx_arg_value); {
-    __pyx_v_value = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int(__pyx_arg_value, PyBUF_WRITABLE); if (unlikely(!__pyx_v_value.memview)) __PYX_ERR(0, 685, __pyx_L3_error)
+    __pyx_v_value = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int(__pyx_arg_value, PyBUF_WRITABLE); if (unlikely(!__pyx_v_value.memview)) __PYX_ERR(0, 697, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("kgraph.utils.read.DataSet.test.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
@@ -11619,27 +11643,27 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
 
-  /* "kgraph/utils/read.pyx":686
+  /* "kgraph/utils/read.pyx":698
  * 
  *         def __set__(self, int[:, ::1] value):
  *             self.testArray = value             # <<<<<<<<<<<<<<
  * 
  *     def __calculate_train_data_size(self):
  */
-  __pyx_t_1 = __pyx_memoryview_fromslice(__pyx_v_value, 2, (PyObject *(*)(char *)) __pyx_memview_get_int, (int (*)(char *, PyObject *)) __pyx_memview_set_int, 0);; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 686, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_fromslice(__pyx_v_value, 2, (PyObject *(*)(char *)) __pyx_memview_get_int, (int (*)(char *, PyObject *)) __pyx_memview_set_int, 0);; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 698, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_PyObject_SetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_testArray, __pyx_t_1) < 0) __PYX_ERR(0, 686, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_testArray, __pyx_t_1) < 0) __PYX_ERR(0, 698, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "kgraph/utils/read.pyx":685
+  /* "kgraph/utils/read.pyx":697
  *             return self.testArray
  * 
  *         def __set__(self, int[:, ::1] value):             # <<<<<<<<<<<<<<
  *             self.testArray = value
  * 
  */
 
@@ -11652,15 +11676,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __PYX_XDEC_MEMVIEW(&__pyx_v_value, 1);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kgraph/utils/read.pyx":688
+/* "kgraph/utils/read.pyx":700
  *             self.testArray = value
  * 
  *     def __calculate_train_data_size(self):             # <<<<<<<<<<<<<<
  *         if self.element_type == 1:
  *             self.train_data_size = self.train_data_ptr.lef_pair_num + self.train_data_ptr.rig_pair_num
  */
 
@@ -11680,72 +11704,72 @@
 static PyObject *__pyx_pf_6kgraph_5utils_4read_7DataSet_22__calculate_train_data_size(struct __pyx_obj_6kgraph_5utils_4read_DataSet *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   __Pyx_RefNannySetupContext("__calculate_train_data_size", 0);
 
-  /* "kgraph/utils/read.pyx":689
+  /* "kgraph/utils/read.pyx":701
  * 
  *     def __calculate_train_data_size(self):
  *         if self.element_type == 1:             # <<<<<<<<<<<<<<
  *             self.train_data_size = self.train_data_ptr.lef_pair_num + self.train_data_ptr.rig_pair_num
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_self->element_type == 1) != 0);
   if (__pyx_t_1) {
 
-    /* "kgraph/utils/read.pyx":690
+    /* "kgraph/utils/read.pyx":702
  *     def __calculate_train_data_size(self):
  *         if self.element_type == 1:
  *             self.train_data_size = self.train_data_ptr.lef_pair_num + self.train_data_ptr.rig_pair_num             # <<<<<<<<<<<<<<
  *         else:
  *             self.train_data_size = self.train_data_ptr.data_size
  */
     __pyx_v_self->train_data_size = (__pyx_v_self->train_data_ptr.lef_pair_num + __pyx_v_self->train_data_ptr.rig_pair_num);
 
-    /* "kgraph/utils/read.pyx":689
+    /* "kgraph/utils/read.pyx":701
  * 
  *     def __calculate_train_data_size(self):
  *         if self.element_type == 1:             # <<<<<<<<<<<<<<
  *             self.train_data_size = self.train_data_ptr.lef_pair_num + self.train_data_ptr.rig_pair_num
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "kgraph/utils/read.pyx":692
+  /* "kgraph/utils/read.pyx":704
  *             self.train_data_size = self.train_data_ptr.lef_pair_num + self.train_data_ptr.rig_pair_num
  *         else:
  *             self.train_data_size = self.train_data_ptr.data_size             # <<<<<<<<<<<<<<
  * 
  *     def set_trainDataSetPair(self, smooth_lambda: float=0.0):
  */
   /*else*/ {
     __pyx_t_2 = __pyx_v_self->train_data_ptr.data_size;
     __pyx_v_self->train_data_size = __pyx_t_2;
   }
   __pyx_L3:;
 
-  /* "kgraph/utils/read.pyx":688
+  /* "kgraph/utils/read.pyx":700
  *             self.testArray = value
  * 
  *     def __calculate_train_data_size(self):             # <<<<<<<<<<<<<<
  *         if self.element_type == 1:
  *             self.train_data_size = self.train_data_ptr.lef_pair_num + self.train_data_ptr.rig_pair_num
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kgraph/utils/read.pyx":694
+/* "kgraph/utils/read.pyx":706
  *             self.train_data_size = self.train_data_ptr.data_size
  * 
  *     def set_trainDataSetPair(self, smooth_lambda: float=0.0):             # <<<<<<<<<<<<<<
  *         '''
  *         smooth_lambda: float, the smooth lambda for the labels in sampling process, default 0.0.
  */
 
@@ -11777,33 +11801,33 @@
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_smooth_lambda);
           if (value) { values[0] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "set_trainDataSetPair") < 0)) __PYX_ERR(0, 694, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "set_trainDataSetPair") < 0)) __PYX_ERR(0, 706, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     if (values[0]) {
-      __pyx_v_smooth_lambda = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_smooth_lambda == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 694, __pyx_L3_error)
+      __pyx_v_smooth_lambda = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_smooth_lambda == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 706, __pyx_L3_error)
     } else {
       __pyx_v_smooth_lambda = ((double)0.0);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("set_trainDataSetPair", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 694, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("set_trainDataSetPair", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 706, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("kgraph.utils.read.DataSet.set_trainDataSetPair", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6kgraph_5utils_4read_7DataSet_24set_trainDataSetPair(((struct __pyx_obj_6kgraph_5utils_4read_DataSet *)__pyx_v_self), __pyx_v_smooth_lambda);
 
@@ -11819,59 +11843,59 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_trainDataSetPair", 0);
 
-  /* "kgraph/utils/read.pyx":699
+  /* "kgraph/utils/read.pyx":711
  *         return the DataSet for DataLoader in pytorch.
  *         '''
  *         self._smooth_lambda = smooth_lambda             # <<<<<<<<<<<<<<
  *         self.element_type = 1
  *         self.__calculate_train_data_size()
  */
   __pyx_v_self->_smooth_lambda = __pyx_v_smooth_lambda;
 
-  /* "kgraph/utils/read.pyx":700
+  /* "kgraph/utils/read.pyx":712
  *         '''
  *         self._smooth_lambda = smooth_lambda
  *         self.element_type = 1             # <<<<<<<<<<<<<<
  *         self.__calculate_train_data_size()
  * 
  */
   __pyx_v_self->element_type = 1;
 
-  /* "kgraph/utils/read.pyx":701
+  /* "kgraph/utils/read.pyx":713
  *         self._smooth_lambda = smooth_lambda
  *         self.element_type = 1
  *         self.__calculate_train_data_size()             # <<<<<<<<<<<<<<
  * 
  *     property smooth_lambda:
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_calculate_train_data_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 701, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_calculate_train_data_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 713, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 701, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 713, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "kgraph/utils/read.pyx":694
+  /* "kgraph/utils/read.pyx":706
  *             self.train_data_size = self.train_data_ptr.data_size
  * 
  *     def set_trainDataSetPair(self, smooth_lambda: float=0.0):             # <<<<<<<<<<<<<<
  *         '''
  *         smooth_lambda: float, the smooth lambda for the labels in sampling process, default 0.0.
  */
 
@@ -11886,15 +11910,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kgraph/utils/read.pyx":704
+/* "kgraph/utils/read.pyx":716
  * 
  *     property smooth_lambda:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return self._smooth_lambda
  * 
  */
 
@@ -11916,29 +11940,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "kgraph/utils/read.pyx":705
+  /* "kgraph/utils/read.pyx":717
  *     property smooth_lambda:
  *         def __get__(self):
  *             return self._smooth_lambda             # <<<<<<<<<<<<<<
  * 
  *         def __set__(self, value: float):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_self->_smooth_lambda); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 705, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_self->_smooth_lambda); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 717, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "kgraph/utils/read.pyx":704
+  /* "kgraph/utils/read.pyx":716
  * 
  *     property smooth_lambda:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return self._smooth_lambda
  * 
  */
 
@@ -11949,15 +11973,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kgraph/utils/read.pyx":707
+/* "kgraph/utils/read.pyx":719
  *             return self._smooth_lambda
  * 
  *         def __set__(self, value: float):             # <<<<<<<<<<<<<<
  *             self._smooth_lambda = value
  *             self.element_type = 1
  */
 
@@ -11968,15 +11992,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
   assert(__pyx_arg_value); {
-    __pyx_v_value = __pyx_PyFloat_AsDouble(__pyx_arg_value); if (unlikely((__pyx_v_value == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 707, __pyx_L3_error)
+    __pyx_v_value = __pyx_PyFloat_AsDouble(__pyx_arg_value); if (unlikely((__pyx_v_value == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 719, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("kgraph.utils.read.DataSet.smooth_lambda.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
@@ -11994,59 +12018,59 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
 
-  /* "kgraph/utils/read.pyx":708
+  /* "kgraph/utils/read.pyx":720
  * 
  *         def __set__(self, value: float):
  *             self._smooth_lambda = value             # <<<<<<<<<<<<<<
  *             self.element_type = 1
  *             self.__calculate_train_data_size()
  */
   __pyx_v_self->_smooth_lambda = __pyx_v_value;
 
-  /* "kgraph/utils/read.pyx":709
+  /* "kgraph/utils/read.pyx":721
  *         def __set__(self, value: float):
  *             self._smooth_lambda = value
  *             self.element_type = 1             # <<<<<<<<<<<<<<
  *             self.__calculate_train_data_size()
  * 
  */
   __pyx_v_self->element_type = 1;
 
-  /* "kgraph/utils/read.pyx":710
+  /* "kgraph/utils/read.pyx":722
  *             self._smooth_lambda = value
  *             self.element_type = 1
  *             self.__calculate_train_data_size()             # <<<<<<<<<<<<<<
  * 
  *     property smooth:
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_calculate_train_data_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 710, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_calculate_train_data_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 722, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 710, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 722, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "kgraph/utils/read.pyx":707
+  /* "kgraph/utils/read.pyx":719
  *             return self._smooth_lambda
  * 
  *         def __set__(self, value: float):             # <<<<<<<<<<<<<<
  *             self._smooth_lambda = value
  *             self.element_type = 1
  */
 
@@ -12060,15 +12084,15 @@
   __Pyx_AddTraceback("kgraph.utils.read.DataSet.smooth_lambda.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kgraph/utils/read.pyx":713
+/* "kgraph/utils/read.pyx":725
  * 
  *     property smooth:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return self._smooth_lambda
  * 
  */
 
@@ -12090,29 +12114,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "kgraph/utils/read.pyx":714
+  /* "kgraph/utils/read.pyx":726
  *     property smooth:
  *         def __get__(self):
  *             return self._smooth_lambda             # <<<<<<<<<<<<<<
  * 
  *         def __set__(self, value: float):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_self->_smooth_lambda); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 714, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_self->_smooth_lambda); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 726, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "kgraph/utils/read.pyx":713
+  /* "kgraph/utils/read.pyx":725
  * 
  *     property smooth:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return self._smooth_lambda
  * 
  */
 
@@ -12123,15 +12147,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kgraph/utils/read.pyx":716
+/* "kgraph/utils/read.pyx":728
  *             return self._smooth_lambda
  * 
  *         def __set__(self, value: float):             # <<<<<<<<<<<<<<
  *             self._smooth_lambda = value
  *             self.element_type = 1
  */
 
@@ -12142,15 +12166,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
   assert(__pyx_arg_value); {
-    __pyx_v_value = __pyx_PyFloat_AsDouble(__pyx_arg_value); if (unlikely((__pyx_v_value == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 716, __pyx_L3_error)
+    __pyx_v_value = __pyx_PyFloat_AsDouble(__pyx_arg_value); if (unlikely((__pyx_v_value == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 728, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("kgraph.utils.read.DataSet.smooth.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
@@ -12168,59 +12192,59 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
 
-  /* "kgraph/utils/read.pyx":717
+  /* "kgraph/utils/read.pyx":729
  * 
  *         def __set__(self, value: float):
  *             self._smooth_lambda = value             # <<<<<<<<<<<<<<
  *             self.element_type = 1
  *             self.__calculate_train_data_size()
  */
   __pyx_v_self->_smooth_lambda = __pyx_v_value;
 
-  /* "kgraph/utils/read.pyx":718
+  /* "kgraph/utils/read.pyx":730
  *         def __set__(self, value: float):
  *             self._smooth_lambda = value
  *             self.element_type = 1             # <<<<<<<<<<<<<<
  *             self.__calculate_train_data_size()
  * 
  */
   __pyx_v_self->element_type = 1;
 
-  /* "kgraph/utils/read.pyx":719
+  /* "kgraph/utils/read.pyx":731
  *             self._smooth_lambda = value
  *             self.element_type = 1
  *             self.__calculate_train_data_size()             # <<<<<<<<<<<<<<
  * 
  *     def get_item_pair(self, index: int):
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_calculate_train_data_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 719, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_calculate_train_data_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 731, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 719, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 731, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "kgraph/utils/read.pyx":716
+  /* "kgraph/utils/read.pyx":728
  *             return self._smooth_lambda
  * 
  *         def __set__(self, value: float):             # <<<<<<<<<<<<<<
  *             self._smooth_lambda = value
  *             self.element_type = 1
  */
 
@@ -12234,15 +12258,15 @@
   __Pyx_AddTraceback("kgraph.utils.read.DataSet.smooth.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kgraph/utils/read.pyx":721
+/* "kgraph/utils/read.pyx":733
  *             self.__calculate_train_data_size()
  * 
  *     def get_item_pair(self, index: int):             # <<<<<<<<<<<<<<
  *         cdef np.ndarray[int, ndim=1] index_per_pair = np.zeros(2, dtype=np.int32)
  *         cdef np.ndarray[float, ndim=1] index_per_label = np.zeros(self.num_ent, dtype=np.float32)
  */
 
@@ -12289,200 +12313,200 @@
   __pyx_pybuffernd_index_per_pair.data = NULL;
   __pyx_pybuffernd_index_per_pair.rcbuffer = &__pyx_pybuffer_index_per_pair;
   __pyx_pybuffer_index_per_label.pybuffer.buf = NULL;
   __pyx_pybuffer_index_per_label.refcount = 0;
   __pyx_pybuffernd_index_per_label.data = NULL;
   __pyx_pybuffernd_index_per_label.rcbuffer = &__pyx_pybuffer_index_per_label;
 
-  /* "kgraph/utils/read.pyx":722
+  /* "kgraph/utils/read.pyx":734
  * 
  *     def get_item_pair(self, index: int):
  *         cdef np.ndarray[int, ndim=1] index_per_pair = np.zeros(2, dtype=np.int32)             # <<<<<<<<<<<<<<
  *         cdef np.ndarray[float, ndim=1] index_per_label = np.zeros(self.num_ent, dtype=np.float32)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 722, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 734, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 722, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 734, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 722, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 734, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 722, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 734, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_int32); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 722, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_int32); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 734, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 722, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 734, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__2, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 722, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__2, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 734, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 722, __pyx_L1_error)
+  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 734, __pyx_L1_error)
   __pyx_t_5 = ((PyArrayObject *)__pyx_t_4);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_index_per_pair.rcbuffer->pybuffer, (PyObject*)__pyx_t_5, &__Pyx_TypeInfo_int, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_index_per_pair = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_index_per_pair.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 722, __pyx_L1_error)
+      __PYX_ERR(0, 734, __pyx_L1_error)
     } else {__pyx_pybuffernd_index_per_pair.diminfo[0].strides = __pyx_pybuffernd_index_per_pair.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_index_per_pair.diminfo[0].shape = __pyx_pybuffernd_index_per_pair.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_5 = 0;
   __pyx_v_index_per_pair = ((PyArrayObject *)__pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "kgraph/utils/read.pyx":723
+  /* "kgraph/utils/read.pyx":735
  *     def get_item_pair(self, index: int):
  *         cdef np.ndarray[int, ndim=1] index_per_pair = np.zeros(2, dtype=np.int32)
  *         cdef np.ndarray[float, ndim=1] index_per_label = np.zeros(self.num_ent, dtype=np.float32)             # <<<<<<<<<<<<<<
  * 
  *         if index < self.train_data_ptr.lef_pair_num:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 723, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_zeros); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 723, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_zeros); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_self->num_ent); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 723, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_self->num_ent); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 723, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_4);
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 723, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 723, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float32); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 723, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float32); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 723, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 735, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 723, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 723, __pyx_L1_error)
+  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 735, __pyx_L1_error)
   __pyx_t_7 = ((PyArrayObject *)__pyx_t_6);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_index_per_label.rcbuffer->pybuffer, (PyObject*)__pyx_t_7, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_index_per_label = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_index_per_label.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 723, __pyx_L1_error)
+      __PYX_ERR(0, 735, __pyx_L1_error)
     } else {__pyx_pybuffernd_index_per_label.diminfo[0].strides = __pyx_pybuffernd_index_per_label.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_index_per_label.diminfo[0].shape = __pyx_pybuffernd_index_per_label.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_7 = 0;
   __pyx_v_index_per_label = ((PyArrayObject *)__pyx_t_6);
   __pyx_t_6 = 0;
 
-  /* "kgraph/utils/read.pyx":725
+  /* "kgraph/utils/read.pyx":737
  *         cdef np.ndarray[float, ndim=1] index_per_label = np.zeros(self.num_ent, dtype=np.float32)
  * 
  *         if index < self.train_data_ptr.lef_pair_num:             # <<<<<<<<<<<<<<
  *             generate_per_pair(&(self.train_data_ptr), self.num_ent, self.num_rel, index_per_pair, index_per_label, index, 0, self._smooth_lambda)
  *         else:
  */
-  __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_self->train_data_ptr.lef_pair_num); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 725, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_self->train_data_ptr.lef_pair_num); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 737, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = PyObject_RichCompare(__pyx_v_index, __pyx_t_6, Py_LT); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 725, __pyx_L1_error)
+  __pyx_t_4 = PyObject_RichCompare(__pyx_v_index, __pyx_t_6, Py_LT); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 737, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 725, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 737, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (__pyx_t_8) {
 
-    /* "kgraph/utils/read.pyx":726
+    /* "kgraph/utils/read.pyx":738
  * 
  *         if index < self.train_data_ptr.lef_pair_num:
  *             generate_per_pair(&(self.train_data_ptr), self.num_ent, self.num_rel, index_per_pair, index_per_label, index, 0, self._smooth_lambda)             # <<<<<<<<<<<<<<
  *         else:
  *             index = index - self.train_data_ptr.lef_pair_num
  */
-    __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_dc_int(((PyObject *)__pyx_v_index_per_pair), PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 726, __pyx_L1_error)
-    __pyx_t_10 = __Pyx_PyObject_to_MemoryviewSlice_dc_float(((PyObject *)__pyx_v_index_per_label), PyBUF_WRITABLE); if (unlikely(!__pyx_t_10.memview)) __PYX_ERR(0, 726, __pyx_L1_error)
-    __pyx_t_11 = __Pyx_PyInt_As_int(__pyx_v_index); if (unlikely((__pyx_t_11 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 726, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_dc_int(((PyObject *)__pyx_v_index_per_pair), PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 738, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_to_MemoryviewSlice_dc_float(((PyObject *)__pyx_v_index_per_label), PyBUF_WRITABLE); if (unlikely(!__pyx_t_10.memview)) __PYX_ERR(0, 738, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyInt_As_int(__pyx_v_index); if (unlikely((__pyx_t_11 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 738, __pyx_L1_error)
     __pyx_f_6kgraph_5utils_4read_generate_per_pair((&__pyx_v_self->train_data_ptr), __pyx_v_self->num_ent, __pyx_v_self->num_rel, __pyx_t_9, __pyx_t_10, __pyx_t_11, 0, __pyx_v_self->_smooth_lambda);
     __PYX_XDEC_MEMVIEW(&__pyx_t_9, 1);
     __pyx_t_9.memview = NULL;
     __pyx_t_9.data = NULL;
     __PYX_XDEC_MEMVIEW(&__pyx_t_10, 1);
     __pyx_t_10.memview = NULL;
     __pyx_t_10.data = NULL;
 
-    /* "kgraph/utils/read.pyx":725
+    /* "kgraph/utils/read.pyx":737
  *         cdef np.ndarray[float, ndim=1] index_per_label = np.zeros(self.num_ent, dtype=np.float32)
  * 
  *         if index < self.train_data_ptr.lef_pair_num:             # <<<<<<<<<<<<<<
  *             generate_per_pair(&(self.train_data_ptr), self.num_ent, self.num_rel, index_per_pair, index_per_label, index, 0, self._smooth_lambda)
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "kgraph/utils/read.pyx":728
+  /* "kgraph/utils/read.pyx":740
  *             generate_per_pair(&(self.train_data_ptr), self.num_ent, self.num_rel, index_per_pair, index_per_label, index, 0, self._smooth_lambda)
  *         else:
  *             index = index - self.train_data_ptr.lef_pair_num             # <<<<<<<<<<<<<<
  *             generate_per_pair(&(self.train_data_ptr), self.num_ent, self.num_rel, index_per_pair, index_per_label, index, 1, self._smooth_lambda)
  *         return index_per_pair, index_per_label
  */
   /*else*/ {
-    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_self->train_data_ptr.lef_pair_num); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 728, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_self->train_data_ptr.lef_pair_num); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 740, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_6 = PyNumber_Subtract(__pyx_v_index, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 728, __pyx_L1_error)
+    __pyx_t_6 = PyNumber_Subtract(__pyx_v_index, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 740, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF_SET(__pyx_v_index, __pyx_t_6);
     __pyx_t_6 = 0;
 
-    /* "kgraph/utils/read.pyx":729
+    /* "kgraph/utils/read.pyx":741
  *         else:
  *             index = index - self.train_data_ptr.lef_pair_num
  *             generate_per_pair(&(self.train_data_ptr), self.num_ent, self.num_rel, index_per_pair, index_per_label, index, 1, self._smooth_lambda)             # <<<<<<<<<<<<<<
  *         return index_per_pair, index_per_label
  * 
  */
-    __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_dc_int(((PyObject *)__pyx_v_index_per_pair), PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 729, __pyx_L1_error)
-    __pyx_t_10 = __Pyx_PyObject_to_MemoryviewSlice_dc_float(((PyObject *)__pyx_v_index_per_label), PyBUF_WRITABLE); if (unlikely(!__pyx_t_10.memview)) __PYX_ERR(0, 729, __pyx_L1_error)
-    __pyx_t_11 = __Pyx_PyInt_As_int(__pyx_v_index); if (unlikely((__pyx_t_11 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 729, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_dc_int(((PyObject *)__pyx_v_index_per_pair), PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 741, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_to_MemoryviewSlice_dc_float(((PyObject *)__pyx_v_index_per_label), PyBUF_WRITABLE); if (unlikely(!__pyx_t_10.memview)) __PYX_ERR(0, 741, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyInt_As_int(__pyx_v_index); if (unlikely((__pyx_t_11 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 741, __pyx_L1_error)
     __pyx_f_6kgraph_5utils_4read_generate_per_pair((&__pyx_v_self->train_data_ptr), __pyx_v_self->num_ent, __pyx_v_self->num_rel, __pyx_t_9, __pyx_t_10, __pyx_t_11, 1, __pyx_v_self->_smooth_lambda);
     __PYX_XDEC_MEMVIEW(&__pyx_t_9, 1);
     __pyx_t_9.memview = NULL;
     __pyx_t_9.data = NULL;
     __PYX_XDEC_MEMVIEW(&__pyx_t_10, 1);
     __pyx_t_10.memview = NULL;
     __pyx_t_10.data = NULL;
   }
   __pyx_L3:;
 
-  /* "kgraph/utils/read.pyx":730
+  /* "kgraph/utils/read.pyx":742
  *             index = index - self.train_data_ptr.lef_pair_num
  *             generate_per_pair(&(self.train_data_ptr), self.num_ent, self.num_rel, index_per_pair, index_per_label, index, 1, self._smooth_lambda)
  *         return index_per_pair, index_per_label             # <<<<<<<<<<<<<<
  * 
  *     def set_trainDataSetTriple(self, num_neg:int, mode: str='all', bern_flag: bool=False):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 730, __pyx_L1_error)
+  __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 742, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_INCREF(((PyObject *)__pyx_v_index_per_pair));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_index_per_pair));
   PyTuple_SET_ITEM(__pyx_t_6, 0, ((PyObject *)__pyx_v_index_per_pair));
   __Pyx_INCREF(((PyObject *)__pyx_v_index_per_label));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_index_per_label));
   PyTuple_SET_ITEM(__pyx_t_6, 1, ((PyObject *)__pyx_v_index_per_label));
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "kgraph/utils/read.pyx":721
+  /* "kgraph/utils/read.pyx":733
  *             self.__calculate_train_data_size()
  * 
  *     def get_item_pair(self, index: int):             # <<<<<<<<<<<<<<
  *         cdef np.ndarray[int, ndim=1] index_per_pair = np.zeros(2, dtype=np.int32)
  *         cdef np.ndarray[float, ndim=1] index_per_label = np.zeros(self.num_ent, dtype=np.float32)
  */
 
@@ -12513,15 +12537,15 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_index_per_label);
   __Pyx_XDECREF(__pyx_v_index);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kgraph/utils/read.pyx":732
+/* "kgraph/utils/read.pyx":744
  *         return index_per_pair, index_per_label
  * 
  *     def set_trainDataSetTriple(self, num_neg:int, mode: str='all', bern_flag: bool=False):             # <<<<<<<<<<<<<<
  *         '''
  *         num_neg: int, the number of negative samples for each positive sample.
  */
 
@@ -12571,15 +12595,15 @@
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_bern_flag);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "set_trainDataSetTriple") < 0)) __PYX_ERR(0, 732, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "set_trainDataSetTriple") < 0)) __PYX_ERR(0, 744, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
@@ -12590,21 +12614,21 @@
     }
     __pyx_v_num_neg = values[0];
     __pyx_v_mode = ((PyObject*)values[1]);
     __pyx_v_bern_flag = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("set_trainDataSetTriple", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 732, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("set_trainDataSetTriple", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 744, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("kgraph.utils.read.DataSet.set_trainDataSetTriple", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_mode), (&PyUnicode_Type), 1, "mode", 1))) __PYX_ERR(0, 732, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_mode), (&PyUnicode_Type), 1, "mode", 1))) __PYX_ERR(0, 744, __pyx_L1_error)
   __pyx_r = __pyx_pf_6kgraph_5utils_4read_7DataSet_28set_trainDataSetTriple(((struct __pyx_obj_6kgraph_5utils_4read_DataSet *)__pyx_v_self), __pyx_v_num_neg, __pyx_v_mode, __pyx_v_bern_flag);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -12625,241 +12649,241 @@
   int __pyx_t_5;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_trainDataSetTriple", 0);
 
-  /* "kgraph/utils/read.pyx":739
+  /* "kgraph/utils/read.pyx":751
  *         return the DataSet for DataLoader in pytorch.
  *         '''
  *         assert mode.lower() in ['all', 'head', 'tail', 'head_tail', 'normal', 'cross'], 'mode must be one of "all", "head", "tail", "head_tail"'             # <<<<<<<<<<<<<<
  *         modes = {'all': 0, 'head': -1, 'tail': 1, 'head_tail': 0, 'normal': 0, 'cross': 2}
  *         mode_i = modes[mode.lower()]
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(!Py_OptimizeFlag)) {
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_mode, __pyx_n_s_lower); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 739, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_mode, __pyx_n_s_lower); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 751, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 739, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 751, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_all, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 739, __pyx_L1_error)
+    __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_all, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 751, __pyx_L1_error)
     if (!__pyx_t_5) {
     } else {
       __pyx_t_4 = __pyx_t_5;
       goto __pyx_L3_bool_binop_done;
     }
-    __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_head, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 739, __pyx_L1_error)
+    __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_head, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 751, __pyx_L1_error)
     if (!__pyx_t_5) {
     } else {
       __pyx_t_4 = __pyx_t_5;
       goto __pyx_L3_bool_binop_done;
     }
-    __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_tail, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 739, __pyx_L1_error)
+    __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_tail, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 751, __pyx_L1_error)
     if (!__pyx_t_5) {
     } else {
       __pyx_t_4 = __pyx_t_5;
       goto __pyx_L3_bool_binop_done;
     }
-    __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_head_tail, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 739, __pyx_L1_error)
+    __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_head_tail, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 751, __pyx_L1_error)
     if (!__pyx_t_5) {
     } else {
       __pyx_t_4 = __pyx_t_5;
       goto __pyx_L3_bool_binop_done;
     }
-    __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_normal, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 739, __pyx_L1_error)
+    __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_normal, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 751, __pyx_L1_error)
     if (!__pyx_t_5) {
     } else {
       __pyx_t_4 = __pyx_t_5;
       goto __pyx_L3_bool_binop_done;
     }
-    __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_cross, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 739, __pyx_L1_error)
+    __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_cross, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 751, __pyx_L1_error)
     __pyx_t_4 = __pyx_t_5;
     __pyx_L3_bool_binop_done:;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (unlikely(!(__pyx_t_4 != 0))) {
       PyErr_SetObject(PyExc_AssertionError, __pyx_kp_u_mode_must_be_one_of_all_head_tai);
-      __PYX_ERR(0, 739, __pyx_L1_error)
+      __PYX_ERR(0, 751, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "kgraph/utils/read.pyx":740
+  /* "kgraph/utils/read.pyx":752
  *         '''
  *         assert mode.lower() in ['all', 'head', 'tail', 'head_tail', 'normal', 'cross'], 'mode must be one of "all", "head", "tail", "head_tail"'
  *         modes = {'all': 0, 'head': -1, 'tail': 1, 'head_tail': 0, 'normal': 0, 'cross': 2}             # <<<<<<<<<<<<<<
  *         mode_i = modes[mode.lower()]
  *         normal_or_cross = 0
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 740, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 752, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_all, __pyx_int_0) < 0) __PYX_ERR(0, 740, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_head, __pyx_int_neg_1) < 0) __PYX_ERR(0, 740, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_tail, __pyx_int_1) < 0) __PYX_ERR(0, 740, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_head_tail, __pyx_int_0) < 0) __PYX_ERR(0, 740, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_normal, __pyx_int_0) < 0) __PYX_ERR(0, 740, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_cross, __pyx_int_2) < 0) __PYX_ERR(0, 740, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_all, __pyx_int_0) < 0) __PYX_ERR(0, 752, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_head, __pyx_int_neg_1) < 0) __PYX_ERR(0, 752, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_tail, __pyx_int_1) < 0) __PYX_ERR(0, 752, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_head_tail, __pyx_int_0) < 0) __PYX_ERR(0, 752, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_normal, __pyx_int_0) < 0) __PYX_ERR(0, 752, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_cross, __pyx_int_2) < 0) __PYX_ERR(0, 752, __pyx_L1_error)
   __pyx_v_modes = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "kgraph/utils/read.pyx":741
+  /* "kgraph/utils/read.pyx":753
  *         assert mode.lower() in ['all', 'head', 'tail', 'head_tail', 'normal', 'cross'], 'mode must be one of "all", "head", "tail", "head_tail"'
  *         modes = {'all': 0, 'head': -1, 'tail': 1, 'head_tail': 0, 'normal': 0, 'cross': 2}
  *         mode_i = modes[mode.lower()]             # <<<<<<<<<<<<<<
  *         normal_or_cross = 0
  *         if mode_i == 2:
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_mode, __pyx_n_s_lower); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 741, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_mode, __pyx_n_s_lower); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 753, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 741, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 753, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyDict_GetItem(__pyx_v_modes, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 741, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_GetItem(__pyx_v_modes, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 753, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_mode_i = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "kgraph/utils/read.pyx":742
+  /* "kgraph/utils/read.pyx":754
  *         modes = {'all': 0, 'head': -1, 'tail': 1, 'head_tail': 0, 'normal': 0, 'cross': 2}
  *         mode_i = modes[mode.lower()]
  *         normal_or_cross = 0             # <<<<<<<<<<<<<<
  *         if mode_i == 2:
  *             mode_i = 1
  */
   __pyx_v_normal_or_cross = 0;
 
-  /* "kgraph/utils/read.pyx":743
+  /* "kgraph/utils/read.pyx":755
  *         mode_i = modes[mode.lower()]
  *         normal_or_cross = 0
  *         if mode_i == 2:             # <<<<<<<<<<<<<<
  *             mode_i = 1
  *             normal_or_cross = 1
  */
-  __pyx_t_2 = __Pyx_PyInt_EqObjC(__pyx_v_mode_i, __pyx_int_2, 2, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 743, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_EqObjC(__pyx_v_mode_i, __pyx_int_2, 2, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 755, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 743, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 755, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__pyx_t_4) {
 
-    /* "kgraph/utils/read.pyx":744
+    /* "kgraph/utils/read.pyx":756
  *         normal_or_cross = 0
  *         if mode_i == 2:
  *             mode_i = 1             # <<<<<<<<<<<<<<
  *             normal_or_cross = 1
  * 
  */
     __Pyx_INCREF(__pyx_int_1);
     __Pyx_DECREF_SET(__pyx_v_mode_i, __pyx_int_1);
 
-    /* "kgraph/utils/read.pyx":745
+    /* "kgraph/utils/read.pyx":757
  *         if mode_i == 2:
  *             mode_i = 1
  *             normal_or_cross = 1             # <<<<<<<<<<<<<<
  * 
  *         self.num_neg = num_neg
  */
     __pyx_v_normal_or_cross = 1;
 
-    /* "kgraph/utils/read.pyx":743
+    /* "kgraph/utils/read.pyx":755
  *         mode_i = modes[mode.lower()]
  *         normal_or_cross = 0
  *         if mode_i == 2:             # <<<<<<<<<<<<<<
  *             mode_i = 1
  *             normal_or_cross = 1
  */
   }
 
-  /* "kgraph/utils/read.pyx":747
+  /* "kgraph/utils/read.pyx":759
  *             normal_or_cross = 1
  * 
  *         self.num_neg = num_neg             # <<<<<<<<<<<<<<
  * 
  *         self.mode = mode_i
  */
-  __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_v_num_neg); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 747, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_v_num_neg); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 759, __pyx_L1_error)
   __pyx_v_self->num_neg = __pyx_t_6;
 
-  /* "kgraph/utils/read.pyx":749
+  /* "kgraph/utils/read.pyx":761
  *         self.num_neg = num_neg
  * 
  *         self.mode = mode_i             # <<<<<<<<<<<<<<
  *         self.normal_or_cross = normal_or_cross
  *         self.bern_flag = int(bern_flag)
  */
-  __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_v_mode_i); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 749, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_v_mode_i); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 761, __pyx_L1_error)
   __pyx_v_self->mode = __pyx_t_6;
 
-  /* "kgraph/utils/read.pyx":750
+  /* "kgraph/utils/read.pyx":762
  * 
  *         self.mode = mode_i
  *         self.normal_or_cross = normal_or_cross             # <<<<<<<<<<<<<<
  *         self.bern_flag = int(bern_flag)
  * 
  */
   __pyx_v_self->normal_or_cross = __pyx_v_normal_or_cross;
 
-  /* "kgraph/utils/read.pyx":751
+  /* "kgraph/utils/read.pyx":763
  *         self.mode = mode_i
  *         self.normal_or_cross = normal_or_cross
  *         self.bern_flag = int(bern_flag)             # <<<<<<<<<<<<<<
  * 
  *         self.train_data_size = self.train_data_ptr.data_size
  */
-  __pyx_t_2 = __Pyx_PyNumber_Int(__pyx_v_bern_flag); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 751, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyNumber_Int(__pyx_v_bern_flag); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 763, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 751, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 763, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_self->bern_flag = __pyx_t_6;
 
-  /* "kgraph/utils/read.pyx":753
+  /* "kgraph/utils/read.pyx":765
  *         self.bern_flag = int(bern_flag)
  * 
  *         self.train_data_size = self.train_data_ptr.data_size             # <<<<<<<<<<<<<<
  * 
  *         self.element_type = 0
  */
   __pyx_t_6 = __pyx_v_self->train_data_ptr.data_size;
   __pyx_v_self->train_data_size = __pyx_t_6;
 
-  /* "kgraph/utils/read.pyx":755
+  /* "kgraph/utils/read.pyx":767
  *         self.train_data_size = self.train_data_ptr.data_size
  * 
  *         self.element_type = 0             # <<<<<<<<<<<<<<
  * 
  *     def set_cross_sampling(self):
  */
   __pyx_v_self->element_type = 0;
 
-  /* "kgraph/utils/read.pyx":732
+  /* "kgraph/utils/read.pyx":744
  *         return index_per_pair, index_per_label
  * 
  *     def set_trainDataSetTriple(self, num_neg:int, mode: str='all', bern_flag: bool=False):             # <<<<<<<<<<<<<<
  *         '''
  *         num_neg: int, the number of negative samples for each positive sample.
  */
 
@@ -12876,15 +12900,15 @@
   __Pyx_XDECREF(__pyx_v_modes);
   __Pyx_XDECREF(__pyx_v_mode_i);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kgraph/utils/read.pyx":757
+/* "kgraph/utils/read.pyx":769
  *         self.element_type = 0
  * 
  *     def set_cross_sampling(self):             # <<<<<<<<<<<<<<
  *         self.mode = 1
  *         self.normal_or_cross = 1
  */
 
@@ -12902,48 +12926,48 @@
 }
 
 static PyObject *__pyx_pf_6kgraph_5utils_4read_7DataSet_30set_cross_sampling(struct __pyx_obj_6kgraph_5utils_4read_DataSet *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_cross_sampling", 0);
 
-  /* "kgraph/utils/read.pyx":758
+  /* "kgraph/utils/read.pyx":770
  * 
  *     def set_cross_sampling(self):
  *         self.mode = 1             # <<<<<<<<<<<<<<
  *         self.normal_or_cross = 1
  * 
  */
   __pyx_v_self->mode = 1;
 
-  /* "kgraph/utils/read.pyx":759
+  /* "kgraph/utils/read.pyx":771
  *     def set_cross_sampling(self):
  *         self.mode = 1
  *         self.normal_or_cross = 1             # <<<<<<<<<<<<<<
  * 
  *     property cross_sampling:
  */
   __pyx_v_self->normal_or_cross = 1;
 
-  /* "kgraph/utils/read.pyx":757
+  /* "kgraph/utils/read.pyx":769
  *         self.element_type = 0
  * 
  *     def set_cross_sampling(self):             # <<<<<<<<<<<<<<
  *         self.mode = 1
  *         self.normal_or_cross = 1
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kgraph/utils/read.pyx":762
+/* "kgraph/utils/read.pyx":774
  * 
  *     property cross_sampling:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return self.normal_or_cross == 1
  * 
  */
 
@@ -12965,29 +12989,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "kgraph/utils/read.pyx":763
+  /* "kgraph/utils/read.pyx":775
  *     property cross_sampling:
  *         def __get__(self):
  *             return self.normal_or_cross == 1             # <<<<<<<<<<<<<<
  * 
  *         def __set__(self, value: bool):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong((__pyx_v_self->normal_or_cross == 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 763, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong((__pyx_v_self->normal_or_cross == 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 775, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "kgraph/utils/read.pyx":762
+  /* "kgraph/utils/read.pyx":774
  * 
  *     property cross_sampling:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return self.normal_or_cross == 1
  * 
  */
 
@@ -12998,15 +13022,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kgraph/utils/read.pyx":765
+/* "kgraph/utils/read.pyx":777
  *             return self.normal_or_cross == 1
  * 
  *         def __set__(self, value: bool):             # <<<<<<<<<<<<<<
  *             if value:
  *                 self.set_cross_sample()
  */
 
@@ -13031,117 +13055,117 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
 
-  /* "kgraph/utils/read.pyx":766
+  /* "kgraph/utils/read.pyx":778
  * 
  *         def __set__(self, value: bool):
  *             if value:             # <<<<<<<<<<<<<<
  *                 self.set_cross_sample()
  *             else:
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_value); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 766, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_value); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 778, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "kgraph/utils/read.pyx":767
+    /* "kgraph/utils/read.pyx":779
  *         def __set__(self, value: bool):
  *             if value:
  *                 self.set_cross_sample()             # <<<<<<<<<<<<<<
  *             else:
  *                 self.mode = 0
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_cross_sample); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 767, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_cross_sample); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 779, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 767, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 779, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "kgraph/utils/read.pyx":766
+    /* "kgraph/utils/read.pyx":778
  * 
  *         def __set__(self, value: bool):
  *             if value:             # <<<<<<<<<<<<<<
  *                 self.set_cross_sample()
  *             else:
  */
     goto __pyx_L3;
   }
 
-  /* "kgraph/utils/read.pyx":769
+  /* "kgraph/utils/read.pyx":781
  *                 self.set_cross_sample()
  *             else:
  *                 self.mode = 0             # <<<<<<<<<<<<<<
  *                 self.normal_or_cross = 0
  *             self.element_type = 0
  */
   /*else*/ {
     __pyx_v_self->mode = 0;
 
-    /* "kgraph/utils/read.pyx":770
+    /* "kgraph/utils/read.pyx":782
  *             else:
  *                 self.mode = 0
  *                 self.normal_or_cross = 0             # <<<<<<<<<<<<<<
  *             self.element_type = 0
  *             self.__calculate_train_data_size()
  */
     __pyx_v_self->normal_or_cross = 0;
   }
   __pyx_L3:;
 
-  /* "kgraph/utils/read.pyx":771
+  /* "kgraph/utils/read.pyx":783
  *                 self.mode = 0
  *                 self.normal_or_cross = 0
  *             self.element_type = 0             # <<<<<<<<<<<<<<
  *             self.__calculate_train_data_size()
  * 
  */
   __pyx_v_self->element_type = 0;
 
-  /* "kgraph/utils/read.pyx":772
+  /* "kgraph/utils/read.pyx":784
  *                 self.normal_or_cross = 0
  *             self.element_type = 0
  *             self.__calculate_train_data_size()             # <<<<<<<<<<<<<<
  * 
  *     property bernoulli_sampling:
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_calculate_train_data_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 772, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_calculate_train_data_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 784, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 772, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 784, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "kgraph/utils/read.pyx":765
+  /* "kgraph/utils/read.pyx":777
  *             return self.normal_or_cross == 1
  * 
  *         def __set__(self, value: bool):             # <<<<<<<<<<<<<<
  *             if value:
  *                 self.set_cross_sample()
  */
 
@@ -13155,15 +13179,15 @@
   __Pyx_AddTraceback("kgraph.utils.read.DataSet.cross_sampling.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kgraph/utils/read.pyx":775
+/* "kgraph/utils/read.pyx":787
  * 
  *     property bernoulli_sampling:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return bool(self.bern_flag)
  * 
  */
 
@@ -13186,33 +13210,33 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "kgraph/utils/read.pyx":776
+  /* "kgraph/utils/read.pyx":788
  *     property bernoulli_sampling:
  *         def __get__(self):
  *             return bool(self.bern_flag)             # <<<<<<<<<<<<<<
  * 
  *         def __set__(self, value: bool):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->bern_flag); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 776, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->bern_flag); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 788, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 776, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 788, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyBool_FromLong((!(!__pyx_t_2))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 776, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong((!(!__pyx_t_2))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 788, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "kgraph/utils/read.pyx":775
+  /* "kgraph/utils/read.pyx":787
  * 
  *     property bernoulli_sampling:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return bool(self.bern_flag)
  * 
  */
 
@@ -13223,15 +13247,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kgraph/utils/read.pyx":778
+/* "kgraph/utils/read.pyx":790
  *             return bool(self.bern_flag)
  * 
  *         def __set__(self, value: bool):             # <<<<<<<<<<<<<<
  *             self.bern_flag = int(value)
  *             self.element_type = 0
  */
 
@@ -13256,63 +13280,63 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
 
-  /* "kgraph/utils/read.pyx":779
+  /* "kgraph/utils/read.pyx":791
  * 
  *         def __set__(self, value: bool):
  *             self.bern_flag = int(value)             # <<<<<<<<<<<<<<
  *             self.element_type = 0
  *             self.__calculate_train_data_size()
  */
-  __pyx_t_1 = __Pyx_PyNumber_Int(__pyx_v_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 779, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyNumber_Int(__pyx_v_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 791, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 779, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 791, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_self->bern_flag = __pyx_t_2;
 
-  /* "kgraph/utils/read.pyx":780
+  /* "kgraph/utils/read.pyx":792
  *         def __set__(self, value: bool):
  *             self.bern_flag = int(value)
  *             self.element_type = 0             # <<<<<<<<<<<<<<
  *             self.__calculate_train_data_size()
  * 
  */
   __pyx_v_self->element_type = 0;
 
-  /* "kgraph/utils/read.pyx":781
+  /* "kgraph/utils/read.pyx":793
  *             self.bern_flag = int(value)
  *             self.element_type = 0
  *             self.__calculate_train_data_size()             # <<<<<<<<<<<<<<
  * 
  *     property num_neg:
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_calculate_train_data_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 781, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_calculate_train_data_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 793, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 781, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 793, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "kgraph/utils/read.pyx":778
+  /* "kgraph/utils/read.pyx":790
  *             return bool(self.bern_flag)
  * 
  *         def __set__(self, value: bool):             # <<<<<<<<<<<<<<
  *             self.bern_flag = int(value)
  *             self.element_type = 0
  */
 
@@ -13326,15 +13350,15 @@
   __Pyx_AddTraceback("kgraph.utils.read.DataSet.bernoulli_sampling.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kgraph/utils/read.pyx":784
+/* "kgraph/utils/read.pyx":796
  * 
  *     property num_neg:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return self.num_neg
  * 
  */
 
@@ -13356,29 +13380,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "kgraph/utils/read.pyx":785
+  /* "kgraph/utils/read.pyx":797
  *     property num_neg:
  *         def __get__(self):
  *             return self.num_neg             # <<<<<<<<<<<<<<
  * 
  *         def __set__(self, value: int):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->num_neg); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 785, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->num_neg); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 797, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "kgraph/utils/read.pyx":784
+  /* "kgraph/utils/read.pyx":796
  * 
  *     property num_neg:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return self.num_neg
  * 
  */
 
@@ -13389,15 +13413,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kgraph/utils/read.pyx":787
+/* "kgraph/utils/read.pyx":799
  *             return self.num_neg
  * 
  *         def __set__(self, value: int):             # <<<<<<<<<<<<<<
  *             self.num_neg = value
  * 
  */
 
@@ -13422,60 +13446,60 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
 
-  /* "kgraph/utils/read.pyx":788
+  /* "kgraph/utils/read.pyx":800
  * 
  *         def __set__(self, value: int):
  *             self.num_neg = value             # <<<<<<<<<<<<<<
  * 
  *             self.element_type = 0
  */
-  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_value); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 788, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_value); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 800, __pyx_L1_error)
   __pyx_v_self->num_neg = __pyx_t_1;
 
-  /* "kgraph/utils/read.pyx":790
+  /* "kgraph/utils/read.pyx":802
  *             self.num_neg = value
  * 
  *             self.element_type = 0             # <<<<<<<<<<<<<<
  *             self.__calculate_train_data_size()
  * 
  */
   __pyx_v_self->element_type = 0;
 
-  /* "kgraph/utils/read.pyx":791
+  /* "kgraph/utils/read.pyx":803
  * 
  *             self.element_type = 0
  *             self.__calculate_train_data_size()             # <<<<<<<<<<<<<<
  * 
  *     def get_item_triple(self, index: int):
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_calculate_train_data_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 791, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_calculate_train_data_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 803, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 791, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 803, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "kgraph/utils/read.pyx":787
+  /* "kgraph/utils/read.pyx":799
  *             return self.num_neg
  * 
  *         def __set__(self, value: int):             # <<<<<<<<<<<<<<
  *             self.num_neg = value
  * 
  */
 
@@ -13489,24 +13513,25 @@
   __Pyx_AddTraceback("kgraph.utils.read.DataSet.num_neg.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kgraph/utils/read.pyx":793
+/* "kgraph/utils/read.pyx":805
  *             self.__calculate_train_data_size()
  * 
  *     def get_item_triple(self, index: int):             # <<<<<<<<<<<<<<
- * 
- *         cdef np.ndarray[int, ndim=1] index_per_triple = np.zeros(3, dtype=np.int32)
+ *         """
+ *         TODO: Generate the triple samples for training.
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_6kgraph_5utils_4read_7DataSet_33get_item_triple(PyObject *__pyx_v_self, PyObject *__pyx_v_index); /*proto*/
+static char __pyx_doc_6kgraph_5utils_4read_7DataSet_32get_item_triple[] = "\n        TODO: Generate the triple samples for training.\n        return triples, labels\n\n        eg.:\n        >>>data = FB15k()\n        >>>samples, labels = data.get_item_triple(1)\n\n        samples:[[[12, 1, 4]]] labels:[[0]]\n\n        eg.:\n        >>>data = FB15k()\n        >>>data.num_neg = 4\n        >>>samples, labels = data.get_item_triple(1)\n\n        samples:[[[12, 1, 5], [12, 1, 138], [0, 1, 5], [12, 1, 7], [12, 1, 4]]]  labels:[[1, 1, -1, 1, 0]]\n\n        In labels, 1 means that replace the head entity, and -1 means that replace the tail entity, and 0 defines the original triple.\n        ";
 static PyObject *__pyx_pw_6kgraph_5utils_4read_7DataSet_33get_item_triple(PyObject *__pyx_v_self, PyObject *__pyx_v_index) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("get_item_triple (wrapper)", 0);
   __pyx_r = __pyx_pf_6kgraph_5utils_4read_7DataSet_32get_item_triple(((struct __pyx_obj_6kgraph_5utils_4read_DataSet *)__pyx_v_self), ((PyObject *)__pyx_v_index));
 
   /* function exit code */
@@ -13554,315 +13579,315 @@
   __pyx_pybuffernd_corrupts.data = NULL;
   __pyx_pybuffernd_corrupts.rcbuffer = &__pyx_pybuffer_corrupts;
   __pyx_pybuffer_index_per_label.pybuffer.buf = NULL;
   __pyx_pybuffer_index_per_label.refcount = 0;
   __pyx_pybuffernd_index_per_label.data = NULL;
   __pyx_pybuffernd_index_per_label.rcbuffer = &__pyx_pybuffer_index_per_label;
 
-  /* "kgraph/utils/read.pyx":795
- *     def get_item_triple(self, index: int):
+  /* "kgraph/utils/read.pyx":826
+ *         """
  * 
  *         cdef np.ndarray[int, ndim=1] index_per_triple = np.zeros(3, dtype=np.int32)             # <<<<<<<<<<<<<<
  *         cdef np.ndarray[int, ndim=2] corrupts = np.zeros((self.num_neg, 3), dtype=np.int32)
  *         cdef np.ndarray[int, ndim=1] index_per_label = np.zeros(self.num_neg + 1, dtype=np.int32)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 795, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 826, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 795, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 826, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 795, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 826, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 795, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 826, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_int32); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 795, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_int32); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 826, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 795, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__3, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 795, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__3, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 826, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 795, __pyx_L1_error)
+  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 826, __pyx_L1_error)
   __pyx_t_5 = ((PyArrayObject *)__pyx_t_4);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_index_per_triple.rcbuffer->pybuffer, (PyObject*)__pyx_t_5, &__Pyx_TypeInfo_int, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_index_per_triple = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_index_per_triple.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 795, __pyx_L1_error)
+      __PYX_ERR(0, 826, __pyx_L1_error)
     } else {__pyx_pybuffernd_index_per_triple.diminfo[0].strides = __pyx_pybuffernd_index_per_triple.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_index_per_triple.diminfo[0].shape = __pyx_pybuffernd_index_per_triple.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_5 = 0;
   __pyx_v_index_per_triple = ((PyArrayObject *)__pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "kgraph/utils/read.pyx":796
+  /* "kgraph/utils/read.pyx":827
  * 
  *         cdef np.ndarray[int, ndim=1] index_per_triple = np.zeros(3, dtype=np.int32)
  *         cdef np.ndarray[int, ndim=2] corrupts = np.zeros((self.num_neg, 3), dtype=np.int32)             # <<<<<<<<<<<<<<
  *         cdef np.ndarray[int, ndim=1] index_per_label = np.zeros(self.num_neg + 1, dtype=np.int32)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 796, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 827, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_zeros); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 796, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_zeros); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 827, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_self->num_neg); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 796, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_self->num_neg); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 827, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 796, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 827, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_4);
   __Pyx_INCREF(__pyx_int_3);
   __Pyx_GIVEREF(__pyx_int_3);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_int_3);
   __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 796, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 827, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 796, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 827, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 796, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 827, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_int32); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 796, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_int32); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 827, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 796, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 827, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 796, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 827, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 796, __pyx_L1_error)
+  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 827, __pyx_L1_error)
   __pyx_t_7 = ((PyArrayObject *)__pyx_t_6);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_corrupts.rcbuffer->pybuffer, (PyObject*)__pyx_t_7, &__Pyx_TypeInfo_int, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_corrupts = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_corrupts.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 796, __pyx_L1_error)
+      __PYX_ERR(0, 827, __pyx_L1_error)
     } else {__pyx_pybuffernd_corrupts.diminfo[0].strides = __pyx_pybuffernd_corrupts.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_corrupts.diminfo[0].shape = __pyx_pybuffernd_corrupts.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_corrupts.diminfo[1].strides = __pyx_pybuffernd_corrupts.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_corrupts.diminfo[1].shape = __pyx_pybuffernd_corrupts.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_t_7 = 0;
   __pyx_v_corrupts = ((PyArrayObject *)__pyx_t_6);
   __pyx_t_6 = 0;
 
-  /* "kgraph/utils/read.pyx":797
+  /* "kgraph/utils/read.pyx":828
  *         cdef np.ndarray[int, ndim=1] index_per_triple = np.zeros(3, dtype=np.int32)
  *         cdef np.ndarray[int, ndim=2] corrupts = np.zeros((self.num_neg, 3), dtype=np.int32)
  *         cdef np.ndarray[int, ndim=1] index_per_label = np.zeros(self.num_neg + 1, dtype=np.int32)             # <<<<<<<<<<<<<<
  * 
  *         index_per_triple[0] = self.train_data_ptr.data[index].head
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 797, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 828, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 797, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 828, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyInt_From_long((__pyx_v_self->num_neg + 1)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 797, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_From_long((__pyx_v_self->num_neg + 1)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 828, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 797, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 828, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_6);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_6);
   __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 797, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 828, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 797, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 828, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_int32); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 797, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_int32); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 828, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 797, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 828, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 797, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 828, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 797, __pyx_L1_error)
+  if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 828, __pyx_L1_error)
   __pyx_t_8 = ((PyArrayObject *)__pyx_t_3);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_index_per_label.rcbuffer->pybuffer, (PyObject*)__pyx_t_8, &__Pyx_TypeInfo_int, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_index_per_label = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_index_per_label.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 797, __pyx_L1_error)
+      __PYX_ERR(0, 828, __pyx_L1_error)
     } else {__pyx_pybuffernd_index_per_label.diminfo[0].strides = __pyx_pybuffernd_index_per_label.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_index_per_label.diminfo[0].shape = __pyx_pybuffernd_index_per_label.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_8 = 0;
   __pyx_v_index_per_label = ((PyArrayObject *)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "kgraph/utils/read.pyx":799
+  /* "kgraph/utils/read.pyx":830
  *         cdef np.ndarray[int, ndim=1] index_per_label = np.zeros(self.num_neg + 1, dtype=np.int32)
  * 
  *         index_per_triple[0] = self.train_data_ptr.data[index].head             # <<<<<<<<<<<<<<
  *         index_per_triple[1] = self.train_data_ptr.data[index].rel
  *         index_per_triple[2] = self.train_data_ptr.data[index].tail
  */
-  __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_v_index); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 799, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_v_index); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 830, __pyx_L1_error)
   __pyx_t_10 = (__pyx_v_self->train_data_ptr.data[__pyx_t_9]).head;
   __pyx_t_11 = 0;
   __pyx_t_12 = -1;
   if (__pyx_t_11 < 0) {
     __pyx_t_11 += __pyx_pybuffernd_index_per_triple.diminfo[0].shape;
     if (unlikely(__pyx_t_11 < 0)) __pyx_t_12 = 0;
   } else if (unlikely(__pyx_t_11 >= __pyx_pybuffernd_index_per_triple.diminfo[0].shape)) __pyx_t_12 = 0;
   if (unlikely(__pyx_t_12 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_12);
-    __PYX_ERR(0, 799, __pyx_L1_error)
+    __PYX_ERR(0, 830, __pyx_L1_error)
   }
   *__Pyx_BufPtrStrided1d(int *, __pyx_pybuffernd_index_per_triple.rcbuffer->pybuffer.buf, __pyx_t_11, __pyx_pybuffernd_index_per_triple.diminfo[0].strides) = __pyx_t_10;
 
-  /* "kgraph/utils/read.pyx":800
+  /* "kgraph/utils/read.pyx":831
  * 
  *         index_per_triple[0] = self.train_data_ptr.data[index].head
  *         index_per_triple[1] = self.train_data_ptr.data[index].rel             # <<<<<<<<<<<<<<
  *         index_per_triple[2] = self.train_data_ptr.data[index].tail
  * 
  */
-  __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_v_index); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 800, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_v_index); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 831, __pyx_L1_error)
   __pyx_t_10 = (__pyx_v_self->train_data_ptr.data[__pyx_t_9]).rel;
   __pyx_t_11 = 1;
   __pyx_t_12 = -1;
   if (__pyx_t_11 < 0) {
     __pyx_t_11 += __pyx_pybuffernd_index_per_triple.diminfo[0].shape;
     if (unlikely(__pyx_t_11 < 0)) __pyx_t_12 = 0;
   } else if (unlikely(__pyx_t_11 >= __pyx_pybuffernd_index_per_triple.diminfo[0].shape)) __pyx_t_12 = 0;
   if (unlikely(__pyx_t_12 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_12);
-    __PYX_ERR(0, 800, __pyx_L1_error)
+    __PYX_ERR(0, 831, __pyx_L1_error)
   }
   *__Pyx_BufPtrStrided1d(int *, __pyx_pybuffernd_index_per_triple.rcbuffer->pybuffer.buf, __pyx_t_11, __pyx_pybuffernd_index_per_triple.diminfo[0].strides) = __pyx_t_10;
 
-  /* "kgraph/utils/read.pyx":801
+  /* "kgraph/utils/read.pyx":832
  *         index_per_triple[0] = self.train_data_ptr.data[index].head
  *         index_per_triple[1] = self.train_data_ptr.data[index].rel
  *         index_per_triple[2] = self.train_data_ptr.data[index].tail             # <<<<<<<<<<<<<<
  * 
  *         generate_per_triple(&(self.train_data_ptr), self.num_ent, self.num_rel, corrupts, index_per_label, index, self.mode, self.normal_or_cross, self.bern_flag)
  */
-  __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_v_index); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 801, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_v_index); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 832, __pyx_L1_error)
   __pyx_t_10 = (__pyx_v_self->train_data_ptr.data[__pyx_t_9]).tail;
   __pyx_t_11 = 2;
   __pyx_t_12 = -1;
   if (__pyx_t_11 < 0) {
     __pyx_t_11 += __pyx_pybuffernd_index_per_triple.diminfo[0].shape;
     if (unlikely(__pyx_t_11 < 0)) __pyx_t_12 = 0;
   } else if (unlikely(__pyx_t_11 >= __pyx_pybuffernd_index_per_triple.diminfo[0].shape)) __pyx_t_12 = 0;
   if (unlikely(__pyx_t_12 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_12);
-    __PYX_ERR(0, 801, __pyx_L1_error)
+    __PYX_ERR(0, 832, __pyx_L1_error)
   }
   *__Pyx_BufPtrStrided1d(int *, __pyx_pybuffernd_index_per_triple.rcbuffer->pybuffer.buf, __pyx_t_11, __pyx_pybuffernd_index_per_triple.diminfo[0].strides) = __pyx_t_10;
 
-  /* "kgraph/utils/read.pyx":803
+  /* "kgraph/utils/read.pyx":834
  *         index_per_triple[2] = self.train_data_ptr.data[index].tail
  * 
  *         generate_per_triple(&(self.train_data_ptr), self.num_ent, self.num_rel, corrupts, index_per_label, index, self.mode, self.normal_or_cross, self.bern_flag)             # <<<<<<<<<<<<<<
  * 
  *         # return index_per_triple, corrupts, index_per_label
  */
-  __pyx_t_13 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int(((PyObject *)__pyx_v_corrupts), PyBUF_WRITABLE); if (unlikely(!__pyx_t_13.memview)) __PYX_ERR(0, 803, __pyx_L1_error)
-  __pyx_t_14 = __Pyx_PyObject_to_MemoryviewSlice_dc_int(((PyObject *)__pyx_v_index_per_label), PyBUF_WRITABLE); if (unlikely(!__pyx_t_14.memview)) __PYX_ERR(0, 803, __pyx_L1_error)
-  __pyx_t_10 = __Pyx_PyInt_As_int(__pyx_v_index); if (unlikely((__pyx_t_10 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 803, __pyx_L1_error)
-  __pyx_f_6kgraph_5utils_4read_generate_per_triple((&__pyx_v_self->train_data_ptr), __pyx_v_self->num_ent, __pyx_v_self->num_rel, __pyx_t_13, __pyx_t_14, __pyx_t_10, __pyx_v_self->mode, __pyx_v_self->normal_or_cross, __pyx_v_self->bern_flag); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 803, __pyx_L1_error)
+  __pyx_t_13 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_int(((PyObject *)__pyx_v_corrupts), PyBUF_WRITABLE); if (unlikely(!__pyx_t_13.memview)) __PYX_ERR(0, 834, __pyx_L1_error)
+  __pyx_t_14 = __Pyx_PyObject_to_MemoryviewSlice_dc_int(((PyObject *)__pyx_v_index_per_label), PyBUF_WRITABLE); if (unlikely(!__pyx_t_14.memview)) __PYX_ERR(0, 834, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyInt_As_int(__pyx_v_index); if (unlikely((__pyx_t_10 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 834, __pyx_L1_error)
+  __pyx_f_6kgraph_5utils_4read_generate_per_triple((&__pyx_v_self->train_data_ptr), __pyx_v_self->num_ent, __pyx_v_self->num_rel, __pyx_t_13, __pyx_t_14, __pyx_t_10, __pyx_v_self->mode, __pyx_v_self->normal_or_cross, __pyx_v_self->bern_flag); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 834, __pyx_L1_error)
   __PYX_XDEC_MEMVIEW(&__pyx_t_13, 1);
   __pyx_t_13.memview = NULL;
   __pyx_t_13.data = NULL;
   __PYX_XDEC_MEMVIEW(&__pyx_t_14, 1);
   __pyx_t_14.memview = NULL;
   __pyx_t_14.data = NULL;
 
-  /* "kgraph/utils/read.pyx":806
+  /* "kgraph/utils/read.pyx":837
  * 
  *         # return index_per_triple, corrupts, index_per_label
  *         index_triples = np.concatenate([corrupts, index_per_triple.reshape((-1, 3))], axis=0)             # <<<<<<<<<<<<<<
  *         return index_triples, index_per_label
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 806, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 837, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_concatenate); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 806, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_concatenate); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 837, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_index_per_triple), __pyx_n_s_reshape); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 806, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_index_per_triple), __pyx_n_s_reshape); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 837, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_3 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_2, __pyx_tuple__4) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_tuple__4);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 806, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 837, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyList_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 806, __pyx_L1_error)
+  __pyx_t_4 = PyList_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 837, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_INCREF(((PyObject *)__pyx_v_corrupts));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_corrupts));
   PyList_SET_ITEM(__pyx_t_4, 0, ((PyObject *)__pyx_v_corrupts));
   __Pyx_GIVEREF(__pyx_t_3);
   PyList_SET_ITEM(__pyx_t_4, 1, __pyx_t_3);
   __pyx_t_3 = 0;
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 806, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 837, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_4);
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 806, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 837, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_axis, __pyx_int_0) < 0) __PYX_ERR(0, 806, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 806, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_axis, __pyx_int_0) < 0) __PYX_ERR(0, 837, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 837, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_index_triples = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "kgraph/utils/read.pyx":807
+  /* "kgraph/utils/read.pyx":838
  *         # return index_per_triple, corrupts, index_per_label
  *         index_triples = np.concatenate([corrupts, index_per_triple.reshape((-1, 3))], axis=0)
  *         return index_triples, index_per_label             # <<<<<<<<<<<<<<
  * 
  *     def __getitem__(self, index: int):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 807, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 838, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_index_triples);
   __Pyx_GIVEREF(__pyx_v_index_triples);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_index_triples);
   __Pyx_INCREF(((PyObject *)__pyx_v_index_per_label));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_index_per_label));
   PyTuple_SET_ITEM(__pyx_t_2, 1, ((PyObject *)__pyx_v_index_per_label));
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "kgraph/utils/read.pyx":793
+  /* "kgraph/utils/read.pyx":805
  *             self.__calculate_train_data_size()
  * 
  *     def get_item_triple(self, index: int):             # <<<<<<<<<<<<<<
- * 
- *         cdef np.ndarray[int, ndim=1] index_per_triple = np.zeros(3, dtype=np.int32)
+ *         """
+ *         TODO: Generate the triple samples for training.
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
@@ -13891,15 +13916,15 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_index_per_label);
   __Pyx_XDECREF(__pyx_v_index_triples);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kgraph/utils/read.pyx":809
+/* "kgraph/utils/read.pyx":840
  *         return index_triples, index_per_label
  * 
  *     def __getitem__(self, index: int):             # <<<<<<<<<<<<<<
  *         index = index % self.train_data_size
  * 
  */
 
@@ -13925,109 +13950,109 @@
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__getitem__", 0);
   __Pyx_INCREF(__pyx_v_index);
 
-  /* "kgraph/utils/read.pyx":810
+  /* "kgraph/utils/read.pyx":841
  * 
  *     def __getitem__(self, index: int):
  *         index = index % self.train_data_size             # <<<<<<<<<<<<<<
  * 
  *         if self.element_type == 0:
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->train_data_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 810, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->train_data_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 841, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyNumber_Remainder(__pyx_v_index, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 810, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Remainder(__pyx_v_index, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 841, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF_SET(__pyx_v_index, __pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "kgraph/utils/read.pyx":812
+  /* "kgraph/utils/read.pyx":843
  *         index = index % self.train_data_size
  * 
  *         if self.element_type == 0:             # <<<<<<<<<<<<<<
  *             return self.get_item_triple(index)
  *         else:
  */
   __pyx_t_3 = ((__pyx_v_self->element_type == 0) != 0);
   if (__pyx_t_3) {
 
-    /* "kgraph/utils/read.pyx":813
+    /* "kgraph/utils/read.pyx":844
  * 
  *         if self.element_type == 0:
  *             return self.get_item_triple(index)             # <<<<<<<<<<<<<<
  *         else:
  *             return self.get_item_pair(index)
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_item_triple); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 813, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_item_triple); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 844, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_1);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
     __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_4, __pyx_v_index) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v_index);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 813, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 844, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
 
-    /* "kgraph/utils/read.pyx":812
+    /* "kgraph/utils/read.pyx":843
  *         index = index % self.train_data_size
  * 
  *         if self.element_type == 0:             # <<<<<<<<<<<<<<
  *             return self.get_item_triple(index)
  *         else:
  */
   }
 
-  /* "kgraph/utils/read.pyx":815
+  /* "kgraph/utils/read.pyx":846
  *             return self.get_item_triple(index)
  *         else:
  *             return self.get_item_pair(index)             # <<<<<<<<<<<<<<
  * 
  *     def __len__(self):
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_item_pair); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 815, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_item_pair); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 846, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_1);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
     __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_4, __pyx_v_index) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v_index);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 815, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 846, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
   }
 
-  /* "kgraph/utils/read.pyx":809
+  /* "kgraph/utils/read.pyx":840
  *         return index_triples, index_per_label
  * 
  *     def __getitem__(self, index: int):             # <<<<<<<<<<<<<<
  *         index = index % self.train_data_size
  * 
  */
 
@@ -14041,15 +14066,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_index);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kgraph/utils/read.pyx":817
+/* "kgraph/utils/read.pyx":848
  *             return self.get_item_pair(index)
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         return self.train_data_size
  */
 
 /* Python wrapper */
@@ -14066,23 +14091,23 @@
 }
 
 static Py_ssize_t __pyx_pf_6kgraph_5utils_4read_7DataSet_36__len__(struct __pyx_obj_6kgraph_5utils_4read_DataSet *__pyx_v_self) {
   Py_ssize_t __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__len__", 0);
 
-  /* "kgraph/utils/read.pyx":818
+  /* "kgraph/utils/read.pyx":849
  * 
  *     def __len__(self):
  *         return self.train_data_size             # <<<<<<<<<<<<<<
  */
   __pyx_r = __pyx_v_self->train_data_size;
   goto __pyx_L0;
 
-  /* "kgraph/utils/read.pyx":817
+  /* "kgraph/utils/read.pyx":848
  *             return self.get_item_pair(index)
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         return self.train_data_size
  */
 
   /* function exit code */
@@ -14341,15 +14366,15 @@
   __Pyx_AddTraceback("kgraph.utils.read.DataSet.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":734
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -14358,29 +14383,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":735
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":736
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 735, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 736, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":734
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -14391,15 +14416,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":737
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -14408,29 +14433,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":738
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":739
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 738, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 739, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":737
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -14441,15 +14466,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":740
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -14458,29 +14483,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":741
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":742
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 741, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 742, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":740
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -14491,15 +14516,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":743
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -14508,29 +14533,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":744
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":745
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 744, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 745, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":743
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -14541,15 +14566,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":746
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -14558,29 +14583,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":747
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":748
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 747, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 748, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":746
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -14591,212 +14616,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":749
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":750
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":751
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":752
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":750
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":753
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":754
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":749
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":868
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":869
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":870
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":931
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":868
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":872
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":873
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":934
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":874
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":875
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":936
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":874
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":876
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":937
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":872
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":880
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -14812,15 +14837,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":881
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -14828,84 +14853,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":882
+      /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":943
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 882, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 943, __pyx_L3_error)
 
-      /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":881
+      /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":883
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":944
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 883, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":884
+      /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 884, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 945, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(3, 884, __pyx_L5_except_error)
+      __PYX_ERR(3, 945, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":881
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":880
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -14920,15 +14945,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":886
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -14944,15 +14969,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":887
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -14960,84 +14985,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":888
+      /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":949
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 888, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 949, __pyx_L3_error)
 
-      /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":887
+      /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":889
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":950
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 889, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":890
+      /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 890, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 951, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(3, 890, __pyx_L5_except_error)
+      __PYX_ERR(3, 951, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":887
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":886
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -15052,15 +15077,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":892
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -15076,15 +15101,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":893
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -15092,84 +15117,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":894
+      /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":955
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 894, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 955, __pyx_L3_error)
 
-      /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":893
+      /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":895
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":956
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 895, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":896
+      /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":957
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 896, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 957, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(3, 896, __pyx_L5_except_error)
+      __PYX_ERR(3, 957, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":893
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":892
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -15184,14 +15209,188 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":967
+ * 
+ * 
+ * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.timedelta64)`
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":979
+ *     bool
+ *     """
+ *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
+  goto __pyx_L0;
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":967
+ * 
+ * 
+ * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.timedelta64)`
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":982
+ * 
+ * 
+ * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.datetime64)`
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("is_datetime64_object", 0);
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":994
+ *     bool
+ *     """
+ *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
+  goto __pyx_L0;
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":982
+ * 
+ * 
+ * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.datetime64)`
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":997
+ * 
+ * 
+ * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy datetime64 object
+ */
+
+static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
+  npy_datetime __pyx_r;
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":1004
+ *     also needed.  That can be found using `get_datetime64_unit`.
+ *     """
+ *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
+  goto __pyx_L0;
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":997
+ * 
+ * 
+ * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy datetime64 object
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":1007
+ * 
+ * 
+ * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ */
+
+static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
+  npy_timedelta __pyx_r;
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":1011
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ *     """
+ *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
+  goto __pyx_L0;
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":1007
+ * 
+ * 
+ * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":1014
+ * 
+ * 
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ */
+
+static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
+  NPY_DATETIMEUNIT __pyx_r;
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":1018
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ *     """
+ *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
+ */
+  __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
+  goto __pyx_L0;
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":1014
+ * 
+ * 
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
 /* "array.pxd":93
  *             __data_union data
  * 
  *         def __getbuffer__(self, Py_buffer* info, int flags):             # <<<<<<<<<<<<<<
  *             # This implementation of getbuffer is geared towards Cython
  *             # requirements, and does not yet fulfill the PEP.
  */
@@ -29430,29 +29629,29 @@
 
 static PyObject *__pyx_getprop_6kgraph_5utils_4read_7DataSet_element_type(PyObject *o, CYTHON_UNUSED void *x) {
   return __pyx_pw_6kgraph_5utils_4read_7DataSet_12element_type_1__get__(o);
 }
 
 static PyMethodDef __pyx_methods_6kgraph_5utils_4read_DataSet[] = {
   {"load", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6kgraph_5utils_4read_7DataSet_3load, METH_VARARGS|METH_KEYWORDS, 0},
-  {"getTrain", (PyCFunction)__pyx_pw_6kgraph_5utils_4read_7DataSet_5getTrain, METH_NOARGS, 0},
-  {"getValid", (PyCFunction)__pyx_pw_6kgraph_5utils_4read_7DataSet_7getValid, METH_NOARGS, 0},
-  {"getTest", (PyCFunction)__pyx_pw_6kgraph_5utils_4read_7DataSet_9getTest, METH_NOARGS, 0},
-  {"getAll", (PyCFunction)__pyx_pw_6kgraph_5utils_4read_7DataSet_11getAll, METH_NOARGS, 0},
+  {"getTrain", (PyCFunction)__pyx_pw_6kgraph_5utils_4read_7DataSet_5getTrain, METH_NOARGS, __pyx_doc_6kgraph_5utils_4read_7DataSet_4getTrain},
+  {"getValid", (PyCFunction)__pyx_pw_6kgraph_5utils_4read_7DataSet_7getValid, METH_NOARGS, __pyx_doc_6kgraph_5utils_4read_7DataSet_6getValid},
+  {"getTest", (PyCFunction)__pyx_pw_6kgraph_5utils_4read_7DataSet_9getTest, METH_NOARGS, __pyx_doc_6kgraph_5utils_4read_7DataSet_8getTest},
+  {"getAll", (PyCFunction)__pyx_pw_6kgraph_5utils_4read_7DataSet_11getAll, METH_NOARGS, __pyx_doc_6kgraph_5utils_4read_7DataSet_10getAll},
   {"resetPosAndNegTest", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6kgraph_5utils_4read_7DataSet_13resetPosAndNegTest, METH_VARARGS|METH_KEYWORDS, 0},
   {"resetPosAndNegValid", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6kgraph_5utils_4read_7DataSet_15resetPosAndNegValid, METH_VARARGS|METH_KEYWORDS, 0},
   {"initConstraint", (PyCFunction)__pyx_pw_6kgraph_5utils_4read_7DataSet_17initConstraint, METH_NOARGS, 0},
   {"resetAllInCache", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6kgraph_5utils_4read_7DataSet_19resetAllInCache, METH_VARARGS|METH_KEYWORDS, 0},
   {"update", (PyCFunction)__pyx_pw_6kgraph_5utils_4read_7DataSet_21update, METH_NOARGS, 0},
   {"__calculate_train_data_size", (PyCFunction)__pyx_pw_6kgraph_5utils_4read_7DataSet_23__calculate_train_data_size, METH_NOARGS, 0},
   {"set_trainDataSetPair", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6kgraph_5utils_4read_7DataSet_25set_trainDataSetPair, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6kgraph_5utils_4read_7DataSet_24set_trainDataSetPair},
   {"get_item_pair", (PyCFunction)__pyx_pw_6kgraph_5utils_4read_7DataSet_27get_item_pair, METH_O, 0},
   {"set_trainDataSetTriple", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6kgraph_5utils_4read_7DataSet_29set_trainDataSetTriple, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6kgraph_5utils_4read_7DataSet_28set_trainDataSetTriple},
   {"set_cross_sampling", (PyCFunction)__pyx_pw_6kgraph_5utils_4read_7DataSet_31set_cross_sampling, METH_NOARGS, 0},
-  {"get_item_triple", (PyCFunction)__pyx_pw_6kgraph_5utils_4read_7DataSet_33get_item_triple, METH_O, 0},
+  {"get_item_triple", (PyCFunction)__pyx_pw_6kgraph_5utils_4read_7DataSet_33get_item_triple, METH_O, __pyx_doc_6kgraph_5utils_4read_7DataSet_32get_item_triple},
   {"__reduce_cython__", (PyCFunction)__pyx_pw_6kgraph_5utils_4read_7DataSet_39__reduce_cython__, METH_NOARGS, 0},
   {"__setstate_cython__", (PyCFunction)__pyx_pw_6kgraph_5utils_4read_7DataSet_41__setstate_cython__, METH_O, 0},
   {0, 0, 0, 0}
 };
 
 static struct PyGetSetDef __pyx_getsets_6kgraph_5utils_4read_DataSet[] = {
   {(char *)"trainArray", __pyx_getprop_6kgraph_5utils_4read_7DataSet_trainArray, __pyx_setprop_6kgraph_5utils_4read_7DataSet_trainArray, (char *)0, 0},
@@ -30339,14 +30538,15 @@
   {&__pyx_n_s_ASCII, __pyx_k_ASCII, sizeof(__pyx_k_ASCII), 0, 0, 1, 1},
   {&__pyx_kp_s_Buffer_view_does_not_expose_stri, __pyx_k_Buffer_view_does_not_expose_stri, sizeof(__pyx_k_Buffer_view_does_not_expose_stri), 0, 0, 1, 0},
   {&__pyx_kp_s_Can_only_create_a_buffer_that_is, __pyx_k_Can_only_create_a_buffer_that_is, sizeof(__pyx_k_Can_only_create_a_buffer_that_is), 0, 0, 1, 0},
   {&__pyx_kp_s_Cannot_assign_to_read_only_memor, __pyx_k_Cannot_assign_to_read_only_memor, sizeof(__pyx_k_Cannot_assign_to_read_only_memor), 0, 0, 1, 0},
   {&__pyx_kp_s_Cannot_create_writable_memory_vi, __pyx_k_Cannot_create_writable_memory_vi, sizeof(__pyx_k_Cannot_create_writable_memory_vi), 0, 0, 1, 0},
   {&__pyx_kp_s_Cannot_index_with_type_s, __pyx_k_Cannot_index_with_type_s, sizeof(__pyx_k_Cannot_index_with_type_s), 0, 0, 1, 0},
   {&__pyx_n_s_DataSet, __pyx_k_DataSet, sizeof(__pyx_k_DataSet), 0, 0, 1, 1},
+  {&__pyx_kp_u_DataSet_get_item_triple_line_805, __pyx_k_DataSet_get_item_triple_line_805, sizeof(__pyx_k_DataSet_get_item_triple_line_805), 0, 1, 0, 0},
   {&__pyx_n_s_Ellipsis, __pyx_k_Ellipsis, sizeof(__pyx_k_Ellipsis), 0, 0, 1, 1},
   {&__pyx_kp_s_Empty_shape_tuple_for_cython_arr, __pyx_k_Empty_shape_tuple_for_cython_arr, sizeof(__pyx_k_Empty_shape_tuple_for_cython_arr), 0, 0, 1, 0},
   {&__pyx_n_s_ImportError, __pyx_k_ImportError, sizeof(__pyx_k_ImportError), 0, 0, 1, 1},
   {&__pyx_kp_s_Incompatible_checksums_s_vs_0xb0, __pyx_k_Incompatible_checksums_s_vs_0xb0, sizeof(__pyx_k_Incompatible_checksums_s_vs_0xb0), 0, 0, 1, 0},
   {&__pyx_n_s_IndexError, __pyx_k_IndexError, sizeof(__pyx_k_IndexError), 0, 0, 1, 1},
   {&__pyx_kp_s_Indirect_dimensions_not_supporte, __pyx_k_Indirect_dimensions_not_supporte, sizeof(__pyx_k_Indirect_dimensions_not_supporte), 0, 0, 1, 0},
   {&__pyx_kp_s_Invalid_mode_expected_c_or_fortr, __pyx_k_Invalid_mode_expected_c_or_fortr, sizeof(__pyx_k_Invalid_mode_expected_c_or_fortr), 0, 0, 1, 0},
@@ -30354,14 +30554,15 @@
   {&__pyx_n_s_MemoryError, __pyx_k_MemoryError, sizeof(__pyx_k_MemoryError), 0, 0, 1, 1},
   {&__pyx_kp_s_MemoryView_of_r_at_0x_x, __pyx_k_MemoryView_of_r_at_0x_x, sizeof(__pyx_k_MemoryView_of_r_at_0x_x), 0, 0, 1, 0},
   {&__pyx_kp_s_MemoryView_of_r_object, __pyx_k_MemoryView_of_r_object, sizeof(__pyx_k_MemoryView_of_r_object), 0, 0, 1, 0},
   {&__pyx_n_b_O, __pyx_k_O, sizeof(__pyx_k_O), 0, 0, 0, 1},
   {&__pyx_kp_s_Out_of_bounds_on_buffer_access_a, __pyx_k_Out_of_bounds_on_buffer_access_a, sizeof(__pyx_k_Out_of_bounds_on_buffer_access_a), 0, 0, 1, 0},
   {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
   {&__pyx_kp_b_T, __pyx_k_T, sizeof(__pyx_k_T), 0, 0, 0, 0},
+  {&__pyx_kp_u_TODO_Generate_the_triple_sample, __pyx_k_TODO_Generate_the_triple_sample, sizeof(__pyx_k_TODO_Generate_the_triple_sample), 0, 1, 0, 0},
   {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
   {&__pyx_kp_s_Unable_to_convert_item_to_object, __pyx_k_Unable_to_convert_item_to_object, sizeof(__pyx_k_Unable_to_convert_item_to_object), 0, 0, 1, 0},
   {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
   {&__pyx_n_s_View_MemoryView, __pyx_k_View_MemoryView, sizeof(__pyx_k_View_MemoryView), 0, 0, 1, 1},
   {&__pyx_kp_b__26, __pyx_k__26, sizeof(__pyx_k__26), 0, 0, 0, 0},
   {&__pyx_kp_b__27, __pyx_k__27, sizeof(__pyx_k__27), 0, 0, 0, 0},
   {&__pyx_kp_b__28, __pyx_k__28, sizeof(__pyx_k__28), 0, 0, 0, 0},
@@ -30495,15 +30696,15 @@
   {&__pyx_n_s_valid_data, __pyx_k_valid_data, sizeof(__pyx_k_valid_data), 0, 0, 1, 1},
   {&__pyx_n_s_zeros, __pyx_k_zeros, sizeof(__pyx_k_zeros), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 39, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(3, 884, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(3, 945, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(4, 109, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(1, 133, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(1, 151, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(1, 404, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(1, 613, __pyx_L1_error)
   __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(1, 832, __pyx_L1_error)
   return 0;
@@ -30511,55 +30712,55 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "kgraph/utils/read.pyx":597
+  /* "kgraph/utils/read.pyx":609
  *             pos_idx = [2 * x for x in idx]
  *             neg_idx = [2 * x + 1 for x in idx]
  *             pos_test_array = test_array[pos_idx, :]             # <<<<<<<<<<<<<<
  *             neg_test_array = test_array[neg_idx, :]
  *             putTestInCache_c(&(self.test_pos_data_ptr), pos_test_array, self.num_ent, self.num_rel, self.tmp_memory_pool)
  */
-  __pyx_slice_ = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice_)) __PYX_ERR(0, 597, __pyx_L1_error)
+  __pyx_slice_ = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice_)) __PYX_ERR(0, 609, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_slice_);
   __Pyx_GIVEREF(__pyx_slice_);
 
-  /* "kgraph/utils/read.pyx":722
+  /* "kgraph/utils/read.pyx":734
  * 
  *     def get_item_pair(self, index: int):
  *         cdef np.ndarray[int, ndim=1] index_per_pair = np.zeros(2, dtype=np.int32)             # <<<<<<<<<<<<<<
  *         cdef np.ndarray[float, ndim=1] index_per_label = np.zeros(self.num_ent, dtype=np.float32)
  * 
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_int_2); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 722, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_int_2); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 734, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "kgraph/utils/read.pyx":795
- *     def get_item_triple(self, index: int):
+  /* "kgraph/utils/read.pyx":826
+ *         """
  * 
  *         cdef np.ndarray[int, ndim=1] index_per_triple = np.zeros(3, dtype=np.int32)             # <<<<<<<<<<<<<<
  *         cdef np.ndarray[int, ndim=2] corrupts = np.zeros((self.num_neg, 3), dtype=np.int32)
  *         cdef np.ndarray[int, ndim=1] index_per_label = np.zeros(self.num_neg + 1, dtype=np.int32)
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_int_3); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 795, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_int_3); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 826, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "kgraph/utils/read.pyx":806
+  /* "kgraph/utils/read.pyx":837
  * 
  *         # return index_per_triple, corrupts, index_per_label
  *         index_triples = np.concatenate([corrupts, index_per_triple.reshape((-1, 3))], axis=0)             # <<<<<<<<<<<<<<
  *         return index_triples, index_per_label
  * 
  */
-  __pyx_tuple__4 = PyTuple_Pack(2, __pyx_int_neg_1, __pyx_int_3); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 806, __pyx_L1_error)
+  __pyx_tuple__4 = PyTuple_Pack(2, __pyx_int_neg_1, __pyx_int_3); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 837, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("self.all_triples_ptr,self.test_data_ptr,self.test_neg_data_ptr,self.test_pos_data_ptr,self.train_data_ptr,self.valid_data_ptr,self.valid_neg_data_ptr,self.valid_pos_data_ptr cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
@@ -30574,33 +30775,33 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self.all_triples_ptr,self.test_data_ptr,self.test_neg_data_ptr,self.test_pos_data_ptr,self.train_data_ptr,self.valid_data_ptr,self.valid_neg_data_ptr,self.valid_pos_data_ptr cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_s_self_all_triples_ptr_self_test_d); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":884
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(3, 884, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(3, 945, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":890
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(3, 890, __pyx_L1_error)
+  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(3, 951, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
   /* "View.MemoryView":133
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
@@ -31066,26 +31267,46 @@
    if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(6, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(7, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 199, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 200, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(3, 199, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(3, 200, __pyx_L1_error)
   __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(3, 222, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(3, 223, __pyx_L1_error)
   __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(3, 226, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(3, 227, __pyx_L1_error)
   __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(3, 238, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(3, 239, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(3, 771, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_number) __PYX_ERR(3, 773, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(3, 775, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(3, 777, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(3, 779, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(3, 781, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(3, 783, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(3, 785, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(3, 787, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_character) __PYX_ERR(3, 789, __pyx_L1_error)
   __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(3, 764, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(3, 827, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("kgraph.utils.memory"); if (unlikely(!__pyx_t_1)) __PYX_ERR(8, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_6kgraph_5utils_6memory_Memory = __Pyx_ImportType(__pyx_t_1, "kgraph.utils.memory", "Memory", sizeof(struct __pyx_obj_6kgraph_5utils_6memory_Memory), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_6kgraph_5utils_6memory_Memory) __PYX_ERR(8, 70, __pyx_L1_error)
   __pyx_ptype_6kgraph_5utils_6memory_Data = __Pyx_ImportType(__pyx_t_1, "kgraph.utils.memory", "Data", sizeof(struct __pyx_obj_6kgraph_5utils_6memory_Data), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_6kgraph_5utils_6memory_Data) __PYX_ERR(8, 75, __pyx_L1_error)
@@ -31439,16 +31660,17 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "kgraph/utils/read.pyx":1
  * # cython: language_level = 3             # <<<<<<<<<<<<<<
  * # distutils: language=c++
  * import numpy as np
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_DataSet_get_item_triple_line_805, __pyx_kp_u_TODO_Generate_the_triple_sample) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test_2, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "View.MemoryView":209
  *         info.obj = self
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_array_getbuffer, "getbuffer(obj, view, flags)")             # <<<<<<<<<<<<<<
```

### Comparing `kgraph-1.0.8/kgraph/utils/read.pxd` & `kgraph-1.0.9/kgraph/utils/read.pxd`

 * *Files identical despite different names*

### Comparing `kgraph-1.0.8/kgraph/utils/read.pyx` & `kgraph-1.0.9/kgraph/utils/read.pyx`

 * *Files 3% similar despite different names*

```diff
@@ -568,26 +568,38 @@
         putValidInCache_c(&(self.valid_data_ptr), valid_data_array, self.num_ent, self.num_rel, self.tmp_memory_pool)
         putTestInCache_c(&(self.test_data_ptr), test_data_array, self.num_ent, self.num_rel, self.tmp_memory_pool)
         putAllInCache_c(&(self.all_triples_ptr), train_data_array, valid_data_array, test_data_array, self.num_ent, self.num_rel, self.tmp_memory_pool)
 
         self.__calculate_train_data_size()
 
     def getTrain(self):
+        """
+        return the array of train data.
+        """
         # global train_data
         return getDataFromCache_c(&(self.train_data_ptr))
     
     def getValid(self):
+        """
+        return the array of valid data.
+        """
         # global valid_data
         return getDataFromCache_c(&(self.valid_data_ptr))
     
     def getTest(self):
+        """
+        return the array of test data.
+        """
         # global test_data
         return getDataFromCache_c(&(self.test_data_ptr))
     
     def getAll(self):
+        """
+        return the array of all data.
+        """
         # global all_triples
         return getDataFromCache_c(&(self.all_triples_ptr))
     
     def resetPosAndNegTest(self, flag=False):
         test_array = self.getTest()
 
         if flag:
@@ -787,14 +799,33 @@
         def __set__(self, value: int):
             self.num_neg = value
 
             self.element_type = 0
             self.__calculate_train_data_size()
     
     def get_item_triple(self, index: int):
+        """
+        TODO: Generate the triple samples for training.
+        return triples, labels
+
+        eg.:
+        >>>data = FB15k()
+        >>>samples, labels = data.get_item_triple(1)
+
+        samples:[[[12, 1, 4]]] labels:[[0]]
+
+        eg.:
+        >>>data = FB15k()
+        >>>data.num_neg = 4
+        >>>samples, labels = data.get_item_triple(1)
+
+        samples:[[[12, 1, 5], [12, 1, 138], [0, 1, 5], [12, 1, 7], [12, 1, 4]]]  labels:[[1, 1, -1, 1, 0]]
+
+        In labels, 1 means that replace the head entity, and -1 means that replace the tail entity, and 0 defines the original triple.
+        """
 
         cdef np.ndarray[int, ndim=1] index_per_triple = np.zeros(3, dtype=np.int32)
         cdef np.ndarray[int, ndim=2] corrupts = np.zeros((self.num_neg, 3), dtype=np.int32)
         cdef np.ndarray[int, ndim=1] index_per_label = np.zeros(self.num_neg + 1, dtype=np.int32)
 
         index_per_triple[0] = self.train_data_ptr.data[index].head
         index_per_triple[1] = self.train_data_ptr.data[index].rel
```

### Comparing `kgraph-1.0.8/kgraph/utils/sample.cpp` & `kgraph-1.0.9/kgraph/utils/sample.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 /* Generated by Cython 0.29.28 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "C:\\ProgramData\\Miniconda3\\include\\Python.h",
-            "C:\\ProgramData\\Miniconda3\\lib\\site-packages\\numpy\\core\\include\\numpy\\arrayobject.h",
-            "C:\\ProgramData\\Miniconda3\\lib\\site-packages\\numpy\\core\\include\\numpy\\ufuncobject.h"
+            "/home/long/miniconda3/include/python3.7m/Python.h",
+            "/home/long/miniconda3/lib/python3.7/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/home/long/miniconda3/lib/python3.7/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/home/long/miniconda3/lib/python3.7/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/home/long/miniconda3/lib/python3.7/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/home/long/miniconda3/lib/python3.7/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "extra_compile_args": [
             "-std=c++11"
         ],
         "include_dirs": [
-            "C:\\ProgramData\\Miniconda3\\lib\\site-packages\\numpy\\core\\include",
-            "C:\\ProgramData\\Miniconda3\\include"
+            "/home/long/miniconda3/lib/python3.7/site-packages/numpy/core/include",
+            "/home/long/miniconda3/include/python3.7m"
         ],
         "language": "c++",
         "name": "kgraph.utils.sample",
         "sources": [
             "kgraph/utils/sample.pyx"
         ]
     },
@@ -720,14 +723,17 @@
 
 #define __PYX_HAVE__kgraph__utils__sample
 #define __PYX_HAVE_API__kgraph__utils__sample
 /* Early includes */
 #include <string.h>
 #include <stdio.h>
 #include "numpy/arrayobject.h"
+#include "numpy/ndarrayobject.h"
+#include "numpy/ndarraytypes.h"
+#include "numpy/arrayscalars.h"
 #include "numpy/ufuncobject.h"
 
     /* NumPy API declarations from "numpy/__init__.pxd" */
     
 #include "ios"
 #include "new"
 #include "stdexcept"
@@ -965,20 +971,20 @@
 #if CYTHON_CCOMPLEX && !defined(__cplusplus) && defined(__sun__) && defined(__GNUC__)
   #undef _Complex_I
   #define _Complex_I 1.0fj
 #endif
 
 
 static const char *__pyx_f[] = {
-  "kgraph\\utils\\sample.pyx",
+  "kgraph/utils/sample.pyx",
   "stringsource",
   "__init__.pxd",
   "type.pxd",
-  "kgraph\\utils\\memory.pxd",
-  "kgraph\\utils\\read.pxd",
+  "kgraph/utils/memory.pxd",
+  "kgraph/utils/read.pxd",
 };
 /* NoFastGil.proto */
 #define __Pyx_PyGILState_Ensure PyGILState_Ensure
 #define __Pyx_PyGILState_Release PyGILState_Release
 #define __Pyx_FastGIL_Remember()
 #define __Pyx_FastGIL_Forget()
 #define __Pyx_FastGilFuncInit()
@@ -1081,195 +1087,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":689
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":690
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":690
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":691
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":691
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":692
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":693
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":696
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":697
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":697
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":698
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":698
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":699
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":700
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":703
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":704
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":704
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":705
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":713
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":714
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":714
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":715
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":715
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":716
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":717
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":718
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":719
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":720
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":721
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":722
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":722
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":723
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":724
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":725
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":726
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1311,42 +1317,42 @@
 struct __pyx_obj_6kgraph_5utils_6sample___pyx_scope_struct_2_generate_pair;
 struct __pyx_obj_6kgraph_5utils_6sample___pyx_scope_struct_3_generate_pair_on_random;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":728
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":729
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":730
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":730
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":732
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":733
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2924,14 +2930,24 @@
 /* Module declarations from 'numpy' */
 
 /* Module declarations from 'numpy' */
 static PyTypeObject *__pyx_ptype_5numpy_dtype = 0;
 static PyTypeObject *__pyx_ptype_5numpy_flatiter = 0;
 static PyTypeObject *__pyx_ptype_5numpy_broadcast = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ndarray = 0;
+static PyTypeObject *__pyx_ptype_5numpy_generic = 0;
+static PyTypeObject *__pyx_ptype_5numpy_number = 0;
+static PyTypeObject *__pyx_ptype_5numpy_integer = 0;
+static PyTypeObject *__pyx_ptype_5numpy_signedinteger = 0;
+static PyTypeObject *__pyx_ptype_5numpy_unsignedinteger = 0;
+static PyTypeObject *__pyx_ptype_5numpy_inexact = 0;
+static PyTypeObject *__pyx_ptype_5numpy_floating = 0;
+static PyTypeObject *__pyx_ptype_5numpy_complexfloating = 0;
+static PyTypeObject *__pyx_ptype_5numpy_flexible = 0;
+static PyTypeObject *__pyx_ptype_5numpy_character = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ufunc = 0;
 
 /* Module declarations from 'libcpp.vector' */
 
 /* Module declarations from 'kgraph.utils.memory' */
 static PyTypeObject *__pyx_ptype_6kgraph_5utils_6memory_Memory = 0;
 static PyTypeObject *__pyx_ptype_6kgraph_5utils_6memory_Data = 0;
@@ -9710,15 +9726,15 @@
   __Pyx_AddTraceback("kgraph.utils.sample.Sample.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":734
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -9727,29 +9743,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":735
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":736
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 735, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 736, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":734
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -9760,15 +9776,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":737
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -9777,29 +9793,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":738
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":739
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 738, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 739, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":737
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -9810,15 +9826,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":740
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -9827,29 +9843,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":741
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":742
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 741, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 742, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":740
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -9860,15 +9876,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":743
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -9877,29 +9893,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":744
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":745
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 744, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 745, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":743
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -9910,15 +9926,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":746
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -9927,29 +9943,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":747
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":748
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 747, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 748, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":746
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -9960,212 +9976,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":749
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":750
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":751
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":752
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":750
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":753
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":754
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":749
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":868
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":869
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":870
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":931
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":868
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":872
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":873
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":934
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":874
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":875
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":936
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":874
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":876
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":937
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":872
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":880
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -10181,15 +10197,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":881
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -10197,84 +10213,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":882
+      /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":943
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 882, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 943, __pyx_L3_error)
 
-      /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":881
+      /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":883
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":944
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 883, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":884
+      /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 884, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 945, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 884, __pyx_L5_except_error)
+      __PYX_ERR(2, 945, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":881
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":880
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -10289,15 +10305,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":886
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -10313,15 +10329,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":887
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -10329,84 +10345,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":888
+      /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":949
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 888, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 949, __pyx_L3_error)
 
-      /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":887
+      /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":889
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":950
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 889, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":890
+      /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 890, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 951, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 890, __pyx_L5_except_error)
+      __PYX_ERR(2, 951, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":887
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":886
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -10421,15 +10437,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":892
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -10445,15 +10461,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":893
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -10461,84 +10477,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":894
+      /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":955
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 894, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 955, __pyx_L3_error)
 
-      /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":893
+      /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":895
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":956
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 895, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":896
+      /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":957
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 896, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 957, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 896, __pyx_L5_except_error)
+      __PYX_ERR(2, 957, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":893
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":892
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -10553,14 +10569,188 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":967
+ * 
+ * 
+ * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.timedelta64)`
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":979
+ *     bool
+ *     """
+ *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
+  goto __pyx_L0;
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":967
+ * 
+ * 
+ * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.timedelta64)`
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":982
+ * 
+ * 
+ * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.datetime64)`
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("is_datetime64_object", 0);
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":994
+ *     bool
+ *     """
+ *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
+  goto __pyx_L0;
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":982
+ * 
+ * 
+ * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.datetime64)`
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":997
+ * 
+ * 
+ * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy datetime64 object
+ */
+
+static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
+  npy_datetime __pyx_r;
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":1004
+ *     also needed.  That can be found using `get_datetime64_unit`.
+ *     """
+ *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
+  goto __pyx_L0;
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":997
+ * 
+ * 
+ * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy datetime64 object
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":1007
+ * 
+ * 
+ * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ */
+
+static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
+  npy_timedelta __pyx_r;
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":1011
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ *     """
+ *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
+  goto __pyx_L0;
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":1007
+ * 
+ * 
+ * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":1014
+ * 
+ * 
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ */
+
+static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
+  NPY_DATETIMEUNIT __pyx_r;
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":1018
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ *     """
+ *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
+ */
+  __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
+  goto __pyx_L0;
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":1014
+ * 
+ * 
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
 /* "View.MemoryView":122
  *         cdef bint dtype_is_object
  * 
  *     def __cinit__(array self, tuple shape, Py_ssize_t itemsize, format not None,             # <<<<<<<<<<<<<<
  *                   mode="c", bint allocate_buffer=True):
  * 
  */
@@ -25467,15 +25657,15 @@
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {&__pyx_n_s_use_shuffle, __pyx_k_use_shuffle, sizeof(__pyx_k_use_shuffle), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 38, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(2, 884, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(2, 945, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(1, 133, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(1, 148, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(1, 151, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(1, 404, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(1, 613, __pyx_L1_error)
   __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(1, 832, __pyx_L1_error)
   return 0;
@@ -25502,33 +25692,33 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self.data_ptr,self.kwargs cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_self_data_ptr_self_kwargs_cannot); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":884
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(2, 884, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(2, 945, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":890
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(2, 890, __pyx_L1_error)
+  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(2, 951, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
   /* "View.MemoryView":133
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
@@ -25973,26 +26163,46 @@
   sizeof(PyTypeObject),
   #else
   sizeof(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 199, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 200, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 199, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 200, __pyx_L1_error)
   __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 222, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 223, __pyx_L1_error)
   __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 226, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 227, __pyx_L1_error)
   __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 239, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 771, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 773, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 775, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 777, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 779, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 781, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 783, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 785, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 787, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 789, __pyx_L1_error)
   __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 764, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 827, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("kgraph.utils.memory"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_6kgraph_5utils_6memory_Memory = __Pyx_ImportType(__pyx_t_1, "kgraph.utils.memory", "Memory", sizeof(struct __pyx_obj_6kgraph_5utils_6memory_Memory), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_6kgraph_5utils_6memory_Memory) __PYX_ERR(4, 70, __pyx_L1_error)
   __pyx_ptype_6kgraph_5utils_6memory_Data = __Pyx_ImportType(__pyx_t_1, "kgraph.utils.memory", "Data", sizeof(struct __pyx_obj_6kgraph_5utils_6memory_Data), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_6kgraph_5utils_6memory_Data) __PYX_ERR(4, 75, __pyx_L1_error)
```

### Comparing `kgraph-1.0.8/kgraph/utils/sample.pyx` & `kgraph-1.0.9/kgraph/utils/sample.pyx`

 * *Files identical despite different names*

### Comparing `kgraph-1.0.8/kgraph/utils/tools.cpp` & `kgraph-1.0.9/kgraph/utils/tools.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 /* Generated by Cython 0.29.28 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "C:\\ProgramData\\Miniconda3\\include\\Python.h",
-            "C:\\ProgramData\\Miniconda3\\lib\\site-packages\\numpy\\core\\include\\numpy\\arrayobject.h",
-            "C:\\ProgramData\\Miniconda3\\lib\\site-packages\\numpy\\core\\include\\numpy\\ufuncobject.h"
+            "/home/long/miniconda3/include/python3.7m/Python.h",
+            "/home/long/miniconda3/lib/python3.7/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/home/long/miniconda3/lib/python3.7/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/home/long/miniconda3/lib/python3.7/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/home/long/miniconda3/lib/python3.7/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/home/long/miniconda3/lib/python3.7/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "extra_compile_args": [
             "-std=c++11"
         ],
         "include_dirs": [
-            "C:\\ProgramData\\Miniconda3\\lib\\site-packages\\numpy\\core\\include",
-            "C:\\ProgramData\\Miniconda3\\include"
+            "/home/long/miniconda3/lib/python3.7/site-packages/numpy/core/include",
+            "/home/long/miniconda3/include/python3.7m"
         ],
         "language": "c++",
         "name": "kgraph.utils.tools",
         "sources": [
             "kgraph/utils/tools.pyx"
         ]
     },
@@ -720,14 +723,17 @@
 
 #define __PYX_HAVE__kgraph__utils__tools
 #define __PYX_HAVE_API__kgraph__utils__tools
 /* Early includes */
 #include <string.h>
 #include <stdio.h>
 #include "numpy/arrayobject.h"
+#include "numpy/ndarrayobject.h"
+#include "numpy/ndarraytypes.h"
+#include "numpy/arrayscalars.h"
 #include "numpy/ufuncobject.h"
 
     /* NumPy API declarations from "numpy/__init__.pxd" */
     
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
@@ -955,15 +961,15 @@
 #if CYTHON_CCOMPLEX && !defined(__cplusplus) && defined(__sun__) && defined(__GNUC__)
   #undef _Complex_I
   #define _Complex_I 1.0fj
 #endif
 
 
 static const char *__pyx_f[] = {
-  "kgraph\\utils\\tools.pyx",
+  "kgraph/utils/tools.pyx",
   "__init__.pxd",
   "type.pxd",
 };
 /* BufferFormatStructs.proto */
 #define IS_UNSIGNED(type) (((type) -1) > 0)
 struct __Pyx_StructField_;
 #define __PYX_BUF_FLAGS_PACKED_STRUCT (1 << 0)
@@ -996,195 +1002,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":689
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":690
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":690
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":691
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":691
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":692
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":693
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":696
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":697
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":697
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":698
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":698
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":699
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":700
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":703
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":704
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":704
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":705
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":713
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":714
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":714
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":715
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":715
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":716
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":717
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":718
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":719
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":720
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":721
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":722
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":722
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":723
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":724
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":725
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":726
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1211,42 +1217,42 @@
     typedef struct { double real, imag; } __pyx_t_double_complex;
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":728
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":729
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":730
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":730
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":732
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":733
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2053,14 +2059,24 @@
 /* Module declarations from 'numpy' */
 
 /* Module declarations from 'numpy' */
 static PyTypeObject *__pyx_ptype_5numpy_dtype = 0;
 static PyTypeObject *__pyx_ptype_5numpy_flatiter = 0;
 static PyTypeObject *__pyx_ptype_5numpy_broadcast = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ndarray = 0;
+static PyTypeObject *__pyx_ptype_5numpy_generic = 0;
+static PyTypeObject *__pyx_ptype_5numpy_number = 0;
+static PyTypeObject *__pyx_ptype_5numpy_integer = 0;
+static PyTypeObject *__pyx_ptype_5numpy_signedinteger = 0;
+static PyTypeObject *__pyx_ptype_5numpy_unsignedinteger = 0;
+static PyTypeObject *__pyx_ptype_5numpy_inexact = 0;
+static PyTypeObject *__pyx_ptype_5numpy_floating = 0;
+static PyTypeObject *__pyx_ptype_5numpy_complexfloating = 0;
+static PyTypeObject *__pyx_ptype_5numpy_flexible = 0;
+static PyTypeObject *__pyx_ptype_5numpy_character = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ufunc = 0;
 
 /* Module declarations from 'kgraph.utils.tools' */
 static __Pyx_TypeInfo __Pyx_TypeInfo_int = { "int", NULL, sizeof(int), { 0 }, 0, IS_UNSIGNED(int) ? 'U' : 'I', IS_UNSIGNED(int), 0 };
 #define __Pyx_MODULE_NAME "kgraph.utils.tools"
 extern int __pyx_module_is_main_kgraph__utils__tools;
 int __pyx_module_is_main_kgraph__utils__tools = 0;
@@ -2193,15 +2209,15 @@
 static const char __pyx_k_entity2id_file_name[] = "entity2id_file_name";
 static const char __pyx_k_generateTripleIdFile[] = "generateTripleIdFile";
 static const char __pyx_k_orignal_triple_files[] = "orignal_triple_files";
 static const char __pyx_k_entity2id_no_sort_txt[] = "entity2id_no_sort.txt";
 static const char __pyx_k_entity2id_on_sort_txt[] = "entity2id_on_sort.txt";
 static const char __pyx_k_relation2id_file_name[] = "relation2id_file_name";
 static const char __pyx_k_from_original_data_dir[] = "from_original_data_dir";
-static const char __pyx_k_kgraph_utils_tools_pyx[] = "kgraph\\utils\\tools.pyx";
+static const char __pyx_k_kgraph_utils_tools_pyx[] = "kgraph/utils/tools.pyx";
 static const char __pyx_k_relation2id_no_sort_txt[] = "relation2id_no_sort.txt";
 static const char __pyx_k_relation2id_on_sort_txt[] = "relation2id_on_sort.txt";
 static const char __pyx_k_load_triple_original_file[] = "load_triple_original_file";
 static const char __pyx_k_numpy_core_multiarray_failed_to[] = "numpy.core.multiarray failed to import";
 static const char __pyx_k_write_triple_from_original_data[] = "write_triple_from_original_data";
 static const char __pyx_k_generateTripleIdFile_locals_lamb[] = "generateTripleIdFile.<locals>.<lambda>";
 static const char __pyx_k_numpy_core_umath_failed_to_impor[] = "numpy.core.umath failed to import";
@@ -9824,15 +9840,15 @@
   __Pyx_XDECREF(__pyx_v_fnn);
   __Pyx_XDECREF(__pyx_v_content);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":734
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -9841,29 +9857,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":735
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":736
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 736, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":734
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -9874,15 +9890,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":737
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -9891,29 +9907,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":738
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":739
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 739, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":737
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -9924,15 +9940,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":740
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -9941,29 +9957,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":741
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":742
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 742, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":740
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -9974,15 +9990,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":743
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -9991,29 +10007,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":744
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":745
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 745, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":743
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -10024,15 +10040,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":746
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -10041,29 +10057,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":747
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":748
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 748, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":746
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -10074,212 +10090,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":749
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":750
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":751
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":752
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":750
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":753
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":754
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":749
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":868
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":869
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":870
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":931
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":868
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":872
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":873
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":934
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":874
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":875
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":936
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":874
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":876
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":937
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":872
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":880
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -10295,15 +10311,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":881
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -10311,84 +10327,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":882
+      /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":943
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 882, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 943, __pyx_L3_error)
 
-      /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":881
+      /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":883
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":944
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 883, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":884
+      /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 884, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 945, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 884, __pyx_L5_except_error)
+      __PYX_ERR(1, 945, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":881
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":880
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -10403,15 +10419,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":886
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -10427,15 +10443,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":887
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -10443,84 +10459,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":888
+      /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":949
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 888, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 949, __pyx_L3_error)
 
-      /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":887
+      /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":889
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":950
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 889, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":890
+      /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 890, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 951, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 890, __pyx_L5_except_error)
+      __PYX_ERR(1, 951, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":887
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":886
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -10535,15 +10551,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":892
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -10559,15 +10575,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":893
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -10575,84 +10591,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":894
+      /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":955
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 894, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 955, __pyx_L3_error)
 
-      /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":893
+      /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":895
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":956
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 895, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":896
+      /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":957
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 896, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 957, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 896, __pyx_L5_except_error)
+      __PYX_ERR(1, 957, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":893
+    /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":892
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -10667,14 +10683,188 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":967
+ * 
+ * 
+ * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.timedelta64)`
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":979
+ *     bool
+ *     """
+ *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
+  goto __pyx_L0;
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":967
+ * 
+ * 
+ * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.timedelta64)`
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":982
+ * 
+ * 
+ * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.datetime64)`
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("is_datetime64_object", 0);
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":994
+ *     bool
+ *     """
+ *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
+  goto __pyx_L0;
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":982
+ * 
+ * 
+ * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.datetime64)`
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":997
+ * 
+ * 
+ * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy datetime64 object
+ */
+
+static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
+  npy_datetime __pyx_r;
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":1004
+ *     also needed.  That can be found using `get_datetime64_unit`.
+ *     """
+ *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
+  goto __pyx_L0;
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":997
+ * 
+ * 
+ * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy datetime64 object
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":1007
+ * 
+ * 
+ * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ */
+
+static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
+  npy_timedelta __pyx_r;
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":1011
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ *     """
+ *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
+  goto __pyx_L0;
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":1007
+ * 
+ * 
+ * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":1014
+ * 
+ * 
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ */
+
+static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
+  NPY_DATETIMEUNIT __pyx_r;
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":1018
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ *     """
+ *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
+ */
+  __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
+  goto __pyx_L0;
+
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":1014
+ * 
+ * 
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
 
 #if PY_MAJOR_VERSION >= 3
 #if CYTHON_PEP489_MULTI_PHASE_INIT
 static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
@@ -10855,15 +11045,15 @@
   {&__pyx_n_s_x, __pyx_k_x, sizeof(__pyx_k_x), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_open = __Pyx_GetBuiltinName(__pyx_n_s_open); if (!__pyx_builtin_open) __PYX_ERR(0, 20, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(0, 129, __pyx_L1_error)
   __pyx_builtin_sorted = __Pyx_GetBuiltinName(__pyx_n_s_sorted); if (!__pyx_builtin_sorted) __PYX_ERR(0, 121, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 884, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 945, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
@@ -10926,33 +11116,33 @@
  * 
  *     valid_index = valid_array[:, 0].isin(train_ent) & valid_array[:, 1].isin(train_rel) & valid_array[:, 2].isin(train_ent)
  */
   __pyx_tuple__9 = PyTuple_Pack(2, __pyx_slice__6, __pyx_int_1); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 140, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":884
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(1, 884, __pyx_L1_error)
+  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(1, 945, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__12);
   __Pyx_GIVEREF(__pyx_tuple__12);
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":890
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(1, 890, __pyx_L1_error)
+  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(1, 951, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__13);
   __Pyx_GIVEREF(__pyx_tuple__13);
 
   /* "kgraph/utils/tools.pyx":9
  * 
  * 
  * def get_str2id(path_data, sep="\t", no_sort=True):             # <<<<<<<<<<<<<<
@@ -11109,26 +11299,46 @@
   sizeof(PyTypeObject),
   #else
   sizeof(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 200, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 200, __pyx_L1_error)
   __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 223, __pyx_L1_error)
   __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 227, __pyx_L1_error)
   __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 239, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 771, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 773, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 775, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 777, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 779, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 781, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 783, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 785, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 787, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 789, __pyx_L1_error)
   __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 764, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 827, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -11486,20 +11696,20 @@
  * import os
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "C:/ProgramData/Miniconda3/lib/site-packages/numpy/__init__.pxd":892
- *         raise ImportError("numpy.core.umath failed to import")
+  /* "../../../../home/long/miniconda3/lib/python3.7/site-packages/numpy/__init__.pxd":1014
  * 
- * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
- *     try:
- *         _import_umath()
+ * 
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
```

### Comparing `kgraph-1.0.8/kgraph/utils/tools.pyx` & `kgraph-1.0.9/kgraph/utils/tools.pyx`

 * *Files identical despite different names*

### Comparing `kgraph-1.0.8/kgraph.egg-info/SOURCES.txt` & `kgraph-1.0.9/kgraph.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -2,27 +2,21 @@
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 kgraph/__init__.py
 kgraph/__init__.pyi
 kgraph/log.py
+kgraph/nn.py
 kgraph.egg-info/PKG-INFO
 kgraph.egg-info/SOURCES.txt
 kgraph.egg-info/dependency_links.txt
 kgraph.egg-info/not-zip-safe
 kgraph.egg-info/requires.txt
 kgraph.egg-info/top_level.txt
-kgraph/utils/classification.cpp
-kgraph/utils/corrupt.cpp
-kgraph/utils/evaluation.cpp
-kgraph/utils/memory.cpp
-kgraph/utils/read.cpp
-kgraph/utils/sample.cpp
-kgraph/utils/tools.cpp
 kgraph/loss/Loss.py
 kgraph/loss/MarginLoss.py
 kgraph/loss/SigmoidLoss.py
 kgraph/loss/SoftplusLoss.py
 kgraph/loss/__init__.py
 kgraph/utils/__init__.py
 kgraph/utils/classification.cpp
```

### Comparing `kgraph-1.0.8/setup.cfg` & `kgraph-1.0.9/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,57 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6465 7363  [metadata]..desc
-00000010: 7269 7074 696f 6e20 3d20 4120 5079 7468  ription = A Pyth
-00000020: 6f6e 206c 6962 7261 7279 2066 6f72 2072  on library for r
-00000030: 656c 6174 696f 6e61 6c20 6c65 6172 6e69  elational learni
-00000040: 6e67 206f 6e20 6b6e 6f77 6c65 6467 6520  ng on knowledge 
-00000050: 6772 6170 6873 2e0d 0a61 7574 686f 7220  graphs...author 
-00000060: 3d20 5368 7561 6e67 6c6f 6e67 2059 616f  = Shuanglong Yao
-00000070: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
-00000080: 2073 6875 616e 676c 6f6e 6779 616f 4067   shuanglongyao@g
-00000090: 6d61 696c 2e63 6f6d 0d0a 6c69 6365 6e73  mail.com..licens
-000000a0: 6520 3d20 4170 6163 6865 2032 2e30 0d0a  e = Apache 2.0..
-000000b0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
-000000c0: 203d 2066 696c 653a 5245 4144 4d45 2e6d   = file:README.m
-000000d0: 640d 0a63 6c61 7373 6966 6965 7273 203d  d..classifiers =
-000000e0: 200d 0a09 4f70 6572 6174 696e 6720 5379   ...Operating Sy
-000000f0: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
-00000100: 656e 6465 6e74 0d0a 0949 6e74 656e 6465  endent...Intende
-00000110: 6420 4175 6469 656e 6365 203a 3a20 4465  d Audience :: De
-00000120: 7665 6c6f 7065 7273 0d0a 0950 726f 6772  velopers...Progr
-00000130: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000140: 3a3a 2043 7974 686f 6e0d 0a09 5072 6f67  :: Cython...Prog
-00000150: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000160: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000170: 370d 0a09 546f 7069 6320 3a3a 2053 6f66  7...Topic :: Sof
-00000180: 7477 6172 6520 4465 7665 6c6f 706d 656e  tware Developmen
-00000190: 7420 3a3a 204c 6962 7261 7269 6573 0d0a  t :: Libraries..
-000001a0: 7072 6f6a 6563 745f 7572 6c73 203d 200d  project_urls = .
-000001b0: 0a09 536f 7572 6365 203d 2068 7474 7073  ..Source = https
-000001c0: 3a2f 2f67 6974 6875 622e 636f 6d2f 5961  ://github.com/Ya
-000001d0: 6f53 6875 616e 672d 6c6f 6e67 2f6b 6772  oShuang-long/kgr
-000001e0: 6170 680d 0a0d 0a5b 6f70 7469 6f6e 735d  aph....[options]
-000001f0: 0d0a 7a69 705f 7361 6665 203d 2046 616c  ..zip_safe = Fal
-00000200: 7365 0d0a 696e 636c 7564 655f 7061 636b  se..include_pack
-00000210: 6167 655f 6461 7461 203d 2046 616c 7365  age_data = False
-00000220: 0d0a 7079 7468 6f6e 5f72 6571 7569 7265  ..python_require
-00000230: 7320 3d20 3e3d 332e 370d 0a69 6e73 7461  s = >=3.7..insta
-00000240: 6c6c 5f72 6571 7569 7265 7320 3d20 0d0a  ll_requires = ..
-00000250: 096e 756d 7079 3e3d 312e 3134 2e33 0d0a  .numpy>=1.14.3..
-00000260: 0974 6f72 6368 3e3d 312e 362e 300d 0a09  .torch>=1.6.0...
-00000270: 7471 646d 3e3d 342e 3233 2e34 0d0a 0970  tqdm>=4.23.4...p
-00000280: 7265 7474 7974 6162 6c65 3e3d 302e 372e  rettytable>=0.7.
-00000290: 320d 0a09 7479 7069 6e67 5f65 7874 656e  2...typing_exten
-000002a0: 7369 6f6e 733e 3d33 2e37 2e30 2c3c 342e  sions>=3.7.0,<4.
-000002b0: 302e 302e 300d 0a0d 0a5b 6264 6973 745f  0.0.0....[bdist_
-000002c0: 7768 6565 6c5d 0d0a 756e 6976 6572 7361  wheel]..universa
-000002d0: 6c20 3d20 4661 6c73 650d 0a0d 0a5b 7364  l = False....[sd
-000002e0: 6973 745d 0d0a 666f 726d 6174 7320 3d20  ist]..formats = 
-000002f0: 677a 7461 720d 0a0d 0a5b 6d79 7079 5d0d  gztar....[mypy].
-00000300: 0a69 676e 6f72 655f 6d69 7373 696e 675f  .ignore_missing_
-00000310: 696d 706f 7274 7320 3d20 5472 7565 0d0a  imports = True..
-00000320: 6967 6e6f 7265 5f6d 6973 7369 6e67 5f69  ignore_missing_i
-00000330: 6d70 6f72 7473 5f70 6572 5f6d 6f64 756c  mports_per_modul
-00000340: 6520 3d20 5472 7565 0d0a 6e6f 5f69 6d70  e = True..no_imp
-00000350: 6c69 6369 745f 6f70 7469 6f6e 616c 203d  licit_optional =
-00000360: 2054 7275 650d 0a61 6c6c 6f77 5f72 6564   True..allow_red
-00000370: 6566 696e 6974 696f 6e20 3d20 5472 7565  efinition = True
-00000380: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
-00000390: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
-000003a0: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
+00000000: 5b6d 6574 6164 6174 615d 0a64 6573 6372  [metadata].descr
+00000010: 6970 7469 6f6e 203d 2041 2050 7974 686f  iption = A Pytho
+00000020: 6e20 6c69 6272 6172 7920 666f 7220 7265  n library for re
+00000030: 6c61 7469 6f6e 616c 206c 6561 726e 696e  lational learnin
+00000040: 6720 6f6e 206b 6e6f 776c 6564 6765 2067  g on knowledge g
+00000050: 7261 7068 732e 0a61 7574 686f 7220 3d20  raphs..author = 
+00000060: 5368 7561 6e67 6c6f 6e67 2059 616f 0a61  Shuanglong Yao.a
+00000070: 7574 686f 725f 656d 6169 6c20 3d20 7368  uthor_email = sh
+00000080: 7561 6e67 6c6f 6e67 7961 6f40 676d 6169  uanglongyao@gmai
+00000090: 6c2e 636f 6d0a 6c69 6365 6e73 6520 3d20  l.com.license = 
+000000a0: 4170 6163 6865 2032 2e30 0a6c 6f6e 675f  Apache 2.0.long_
+000000b0: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
+000000c0: 6c65 3a52 4541 444d 452e 6d64 0a63 6c61  le:README.md.cla
+000000d0: 7373 6966 6965 7273 203d 200a 094f 7065  ssifiers = ..Ope
+000000e0: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
+000000f0: 204f 5320 496e 6465 7065 6e64 656e 740a   OS Independent.
+00000100: 0949 6e74 656e 6465 6420 4175 6469 656e  .Intended Audien
+00000110: 6365 203a 3a20 4465 7665 6c6f 7065 7273  ce :: Developers
+00000120: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
+00000130: 6e67 7561 6765 203a 3a20 4379 7468 6f6e  nguage :: Cython
+00000140: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
+00000150: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000160: 203a 3a20 332e 370a 0954 6f70 6963 203a   :: 3.7..Topic :
+00000170: 3a20 536f 6674 7761 7265 2044 6576 656c  : Software Devel
+00000180: 6f70 6d65 6e74 203a 3a20 4c69 6272 6172  opment :: Librar
+00000190: 6965 730a 7072 6f6a 6563 745f 7572 6c73  ies.project_urls
+000001a0: 203d 200a 0953 6f75 7263 6520 3d20 6874   = ..Source = ht
+000001b0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000001c0: 2f59 616f 5368 7561 6e67 2d6c 6f6e 672f  /YaoShuang-long/
+000001d0: 6b67 7261 7068 0a0a 5b6f 7074 696f 6e73  kgraph..[options
+000001e0: 5d0a 7a69 705f 7361 6665 203d 2046 616c  ].zip_safe = Fal
+000001f0: 7365 0a69 6e63 6c75 6465 5f70 6163 6b61  se.include_packa
+00000200: 6765 5f64 6174 6120 3d20 4661 6c73 650a  ge_data = False.
+00000210: 7079 7468 6f6e 5f72 6571 7569 7265 7320  python_requires 
+00000220: 3d20 3e3d 332e 370a 696e 7374 616c 6c5f  = >=3.7.install_
+00000230: 7265 7175 6972 6573 203d 200a 096e 756d  requires = ..num
+00000240: 7079 3e3d 312e 3134 2e33 0a09 746f 7263  py>=1.14.3..torc
+00000250: 683e 3d31 2e36 2e30 0a09 7471 646d 3e3d  h>=1.6.0..tqdm>=
+00000260: 342e 3233 2e34 0a09 7072 6574 7479 7461  4.23.4..prettyta
+00000270: 626c 653e 3d30 2e37 2e32 0a09 7479 7069  ble>=0.7.2..typi
+00000280: 6e67 5f65 7874 656e 7369 6f6e 733e 3d33  ng_extensions>=3
+00000290: 2e37 2e30 2c3c 342e 302e 302e 300a 0a5b  .7.0,<4.0.0.0..[
+000002a0: 6264 6973 745f 7768 6565 6c5d 0a75 6e69  bdist_wheel].uni
+000002b0: 7665 7273 616c 203d 2046 616c 7365 0a0a  versal = False..
+000002c0: 5b73 6469 7374 5d0a 666f 726d 6174 7320  [sdist].formats 
+000002d0: 3d20 677a 7461 720a 0a5b 6d79 7079 5d0a  = gztar..[mypy].
+000002e0: 6967 6e6f 7265 5f6d 6973 7369 6e67 5f69  ignore_missing_i
+000002f0: 6d70 6f72 7473 203d 2054 7275 650a 6967  mports = True.ig
+00000300: 6e6f 7265 5f6d 6973 7369 6e67 5f69 6d70  nore_missing_imp
+00000310: 6f72 7473 5f70 6572 5f6d 6f64 756c 6520  orts_per_module 
+00000320: 3d20 5472 7565 0a6e 6f5f 696d 706c 6963  = True.no_implic
+00000330: 6974 5f6f 7074 696f 6e61 6c20 3d20 5472  it_optional = Tr
+00000340: 7565 0a61 6c6c 6f77 5f72 6564 6566 696e  ue.allow_redefin
+00000350: 6974 696f 6e20 3d20 5472 7565 0a0a 5b65  ition = True..[e
+00000360: 6767 5f69 6e66 6f5d 0a74 6167 5f62 7569  gg_info].tag_bui
+00000370: 6c64 203d 200a 7461 675f 6461 7465 203d  ld = .tag_date =
+00000380: 2030 0a0a                                 0..
```

### Comparing `kgraph-1.0.8/setup.py` & `kgraph-1.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -57,22 +57,16 @@
 }
 
 
 def is_new_osx():
     """Check whether we're on OSX >= 10.7"""
     if sys.platform != "darwin":
         return False
-    mac_ver = platform.mac_ver()[0]
-    if mac_ver.startswith("10"):
-        minor_version = int(mac_ver.split(".")[1])
-        if minor_version >= 7:
-            return True
-        else:
-            return False
-    return False
+    major_version, minor_version, _ = platform.mac_ver(release_level=0)
+    return int(major_version) > 10 or (int(major_version) == 10 and int(minor_version) >= 7)
 
 
 if is_new_osx():
     # On Mac, use libc++ because Apple deprecated use of
     # libstdc
     COMPILE_OPTIONS["other"].append("-stdlib=libc++")
     LINK_OPTIONS["other"].append("-lc++")
@@ -80,74 +74,84 @@
     # See: https://stackoverflow.com/questions/1653047/avoid-linking-to-libstdc
     LINK_OPTIONS["other"].append("-nodefaultlibs")
 
 # By subclassing build_extensions we have the actual compiler that will be used which is really known only after finalize_options
 # http://stackoverflow.com/questions/724664/python-distutils-how-to-get-a-compiler-that-is-going-to-be-used
 class build_ext_options:
     def build_options(self):
+        """
+        Builds compile and link options for the current compiler type and applies them to each extension.
+        
+        :return: None
+        """
+        compile_options = COMPILE_OPTIONS.get(
+            self.compiler.compiler_type, COMPILE_OPTIONS["other"]
+        )
+        link_options = LINK_OPTIONS.get(
+            self.compiler.compiler_type, LINK_OPTIONS["other"]
+        )
         for e in self.extensions:
-            e.extra_compile_args += COMPILE_OPTIONS.get(
-                self.compiler.compiler_type, COMPILE_OPTIONS["other"]
-            )
-        for e in self.extensions:
-            e.extra_link_args += LINK_OPTIONS.get(
-                self.compiler.compiler_type, LINK_OPTIONS["other"]
-            )
+            e.extra_compile_args += compile_options
+            e.extra_link_args += link_options
 
 
 class build_ext_subclass(build_ext, build_ext_options):
     def build_extensions(self):
         build_ext_options.build_options(self)
         build_ext.build_extensions(self)
 
 
 def clean(path):
-    for path in path.glob("**/*"):
-        if path.is_file() and path.suffix in (".so", ".cpp", ".pyd", ".html"):
-            print(f"Deleting {path.name}")
-            path.unlink()
+    """
+    Deletes all the files with certain suffixes within the directory and its subdirectories.
+    
+    :param path: The directory path to clean up.
+    :type path: Path object
+    
+    :return: None
+    """
+    to_delete = [p for p in path.glob("**/*") if p.is_file() and p.suffix in (".so", ".cpp", ".pyd", ".html")]
+    for p in to_delete:
+        try:
+            p.unlink()
+            print(f"Deleted {p.name}")
+        except PermissionError:
+            print(f"Permission denied for {p.name}")
 
 def setup_package():
-    # write_git_info_py()
     if len(sys.argv) > 1 and sys.argv[1] == "clean":
         return clean(PACKAGE_ROOT)
-    
-    root = os.getcwd()
-    if not os.path.exists(os.path.join(root, "kgraph", "package")):
-        os.makedirs(os.path.join(root, "kgraph", "package"))
 
-    for copy_file, target_dir in COPY_FILES.items():
-        if copy_file.exists():
-            shutil.copy(str(copy_file), str(target_dir))
-            print(f"Copied {copy_file} -> {target_dir}")
+    copy_files()
+
+    include_dirs = [np.get_include(), get_python_inc(plat_specific=True)]
+    ext_modules = [Extension(
+        name,
+        [name.replace(".", "/") + ".pyx"],
+        language='c++',
+        include_dirs=include_dirs,
+        extra_compile_args=["-std=c++11"]) for name in MOD_NAMES]
 
-    include_dirs = [
-        np.get_include(),
-        get_python_inc(plat_specific=True),
-    ]
-    ext_modules = []
-    for name in MOD_NAMES:
-        mod_path = name.replace(".", "/") + ".pyx"
-        ext = Extension(
-            name, [mod_path], language='c++', include_dirs=include_dirs, extra_compile_args=["-std=c++11"]
-        )
-        ext_modules.append(ext)
     print("Cythonizing sources")
     ext_modules = cythonize(ext_modules, compiler_directives=COMPILER_DIRECTIVES)
-    # ext_modules = cythonize(ext_modules, language_level=3)
 
     setup(
         name="kgraph",
         packages=PACKAGES,
-        version="1.0.8",
+        version="1.0.9",
         ext_modules=ext_modules,
         cmdclass={"build_ext": build_ext_subclass},
-        package_data={"": ["*.pyx", "*.pxd", "*.pxi"]},
-    )
-    
-    # clean(PACKAGE_ROOT)
-    
-    # shutil.copy(os.path.join("./", "test.py"), os.path.join("./", "build", "lib.lib.win-amd64-3.7"))
+        package_data={"": ["*.pyx", "*.pxd", "*.pxi"]})
+
+def copy_files():
+    root = os.getcwd()
+    package_dir = os.path.join(root, "kgraph", "package")
+    os.makedirs(package_dir, exist_ok=True)
+
+    for copy_file, target_dir in COPY_FILES.items():
+        if copy_file.exists():
+            shutil.copy(str(copy_file), str(target_dir))
+            print(f"Copied {copy_file} -> {target_dir}")
 
 
 if __name__ == "__main__":
     setup_package()
```

