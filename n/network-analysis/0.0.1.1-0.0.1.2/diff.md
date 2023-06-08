# Comparing `tmp/network-analysis-0.0.1.1.tar.gz` & `tmp/network-analysis-0.0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "network-analysis-0.0.1.1.tar", last modified: Mon May 15 01:23:44 2023, max compression
+gzip compressed data, was "network-analysis-0.0.1.2.tar", last modified: Thu Jun  8 20:43:10 2023, max compression
```

## Comparing `network-analysis-0.0.1.1.tar` & `network-analysis-0.0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:23:44.913929 network-analysis-0.0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-15 01:23:28.000000 network-analysis-0.0.1.1/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-15 01:23:44.913929 network-analysis-0.0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 01:23:28.000000 network-analysis-0.0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-15 01:23:28.000000 network-analysis-0.0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 01:23:44.913929 network-analysis-0.0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:23:44.913929 network-analysis-0.0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:23:44.913929 network-analysis-0.0.1.1/src/network_analysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-15 01:23:44.000000 network-analysis-0.0.1.1/src/network_analysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-15 01:23:44.000000 network-analysis-0.0.1.1/src/network_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 01:23:44.000000 network-analysis-0.0.1.1/src/network_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 01:23:44.000000 network-analysis-0.0.1.1/src/network_analysis.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:23:44.913929 network-analysis-0.0.1.1/src/networkanalysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 01:23:28.000000 network-analysis-0.0.1.1/src/networkanalysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:23:44.913929 network-analysis-0.0.1.1/src/networkanalysis/ergm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 01:23:28.000000 network-analysis-0.0.1.1/src/networkanalysis/ergm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-05-15 01:23:28.000000 network-analysis-0.0.1.1/src/networkanalysis/ergm/simulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-05-15 01:23:28.000000 network-analysis-0.0.1.1/src/networkanalysis/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:23:44.913929 network-analysis-0.0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-05-15 01:23:28.000000 network-analysis-0.0.1.1/tests/test_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:10.171674 network-analysis-0.0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-08 20:43:00.000000 network-analysis-0.0.1.2/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-08 20:43:10.171674 network-analysis-0.0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:00.000000 network-analysis-0.0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-08 20:43:00.000000 network-analysis-0.0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 20:43:10.171674 network-analysis-0.0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:10.171674 network-analysis-0.0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:10.171674 network-analysis-0.0.1.2/src/network_analysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-08 20:43:10.000000 network-analysis-0.0.1.2/src/network_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-08 20:43:10.000000 network-analysis-0.0.1.2/src/network_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 20:43:10.000000 network-analysis-0.0.1.2/src/network_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 20:43:10.000000 network-analysis-0.0.1.2/src/network_analysis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:10.171674 network-analysis-0.0.1.2/src/networkanalysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:00.000000 network-analysis-0.0.1.2/src/networkanalysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:10.171674 network-analysis-0.0.1.2/src/networkanalysis/ergm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:00.000000 network-analysis-0.0.1.2/src/networkanalysis/ergm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-06-08 20:43:00.000000 network-analysis-0.0.1.2/src/networkanalysis/ergm/simulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-06-08 20:43:00.000000 network-analysis-0.0.1.2/src/networkanalysis/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:10.171674 network-analysis-0.0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-06-08 20:43:00.000000 network-analysis-0.0.1.2/tests/test_statistics.py
```

### Comparing `network-analysis-0.0.1.1/LICENCE` & `network-analysis-0.0.1.2/LICENCE`

 * *Files identical despite different names*

### Comparing `network-analysis-0.0.1.1/PKG-INFO` & `network-analysis-0.0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: network-analysis
-Version: 0.0.1.1
+Version: 0.0.1.2
 Summary: Work in progress...
 Author-email: Gabriel Fortin-Leblanc <gabriel.fortin-leblanc@umontreal.ca>
 Project-URL: Homepage, https://github.com/gabriel-fortin-leblanc/network-analysis
 Project-URL: Bug Tracker, https://github.com/gabriel-fortin-leblanc/network-analysis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `network-analysis-0.0.1.1/pyproject.toml` & `network-analysis-0.0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "network-analysis"
-version = "0.0.1.1"
+version = "0.0.1.2"
 authors = [
   { name="Gabriel Fortin-Leblanc", email="gabriel.fortin-leblanc@umontreal.ca" },
 ]
 description = "Work in progress..."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `network-analysis-0.0.1.1/src/network_analysis.egg-info/PKG-INFO` & `network-analysis-0.0.1.2/src/network_analysis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: network-analysis
-Version: 0.0.1.1
+Version: 0.0.1.2
 Summary: Work in progress...
 Author-email: Gabriel Fortin-Leblanc <gabriel.fortin-leblanc@umontreal.ca>
 Project-URL: Homepage, https://github.com/gabriel-fortin-leblanc/network-analysis
 Project-URL: Bug Tracker, https://github.com/gabriel-fortin-leblanc/network-analysis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `network-analysis-0.0.1.1/src/networkanalysis/statistics.py` & `network-analysis-0.0.1.2/src/networkanalysis/statistics.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """This module contains classes and functions to compute statistics on
 networks.
 """
+import copy
+from collections import OrderedDict
 from typing import Any
 
 import networkx as nx
 import numpy as np
 from scipy.special import comb
 
 
@@ -100,15 +102,14 @@
 
     :param graph: The graph.
     :type graph: NetworkX graph.
     :return: The number of mutual connections.
     :rtype: Integer.
     """
     adj = nx.to_numpy_array(graph)
-    print(adj)
     upper_diag_idx = np.triu_indices(adj.shape[0], 1)
     count_edges = adj[upper_diag_idx] + adj.T[upper_diag_idx]
     if not nx.is_directed(graph):
         count_edges /= 2
     return (count_edges > 1).sum()
 
 
@@ -176,20 +177,57 @@
         return mutuals(graph)
 
 
 def stats_transform(stats):
     """Transform the list of statistics into one function that computes the
     vector of statistics from the list.
 
-    :param stats: List of callable object that takes a NetworkX graph as argument.
+    :param stats: List of callable object that takes a NetworkX graph as
+        argument.
     :type stats: List.
     """
 
     def stats_comp(graph):
         graph_stats = np.empty(
             (len(stats)),
         )
         for i, stat in enumerate(stats):
             graph_stats[i] = stat(graph)
         return graph_stats
 
     return stats_comp
+
+
+class StatsComp:
+    def __init__(self, stats):
+        if isinstance(stats, StatsComp):
+            self._func = stats._func
+            self._len = stats._len
+        else:
+            self._func = stats_transform(stats)
+            self._len = len(stats)
+
+    def __len__(self):
+        return self._len
+
+    def __call__(self, graph):
+        return self._func(graph)
+
+
+class CachedStatsComp(StatsComp):
+    def __init__(self, stats, max_size=10000):
+        super().__init__(stats)
+
+        self._cache = OrderedDict()
+        if isinstance(stats, CachedStatsComp):
+            self._cache.update(stats._cache)
+        self._max_size = max_size
+
+    def __call__(self, graph):
+        if graph in self._cache:
+            return self._cache[graph]
+
+        if len(self._cache) >= self._max_size:
+            self._cache.popitem()
+        stats = self._func(graph)
+        self._cache[graph] = stats
+        return stats
```

