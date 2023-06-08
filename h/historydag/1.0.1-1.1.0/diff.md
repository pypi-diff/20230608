# Comparing `tmp/historydag-1.0.1.tar.gz` & `tmp/historydag-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "historydag-1.0.1.tar", last modified: Wed Jul  6 14:47:09 2022, max compression
+gzip compressed data, was "historydag-1.1.0.tar", last modified: Thu Jun  8 18:46:24 2023, max compression
```

## Comparing `historydag-1.0.1.tar` & `historydag-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 14:47:09.844558 historydag-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)    35141 2022-07-06 14:47:00.000000 historydag-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-07-06 14:47:00.000000 historydag-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4353 2022-07-06 14:47:09.844558 historydag-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3904 2022-07-06 14:47:00.000000 historydag-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 14:47:09.848558 historydag-1.0.1/historydag/
--rw-r--r--   0 runner    (1001) docker     (121)      278 2022-07-06 14:47:00.000000 historydag-1.0.1/historydag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-07-06 14:47:09.848558 historydag-1.0.1/historydag/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     1022 2022-07-06 14:47:00.000000 historydag-1.0.1/historydag/counterops.py
--rw-r--r--   0 runner    (1001) docker     (121)    70187 2022-07-06 14:47:00.000000 historydag-1.0.1/historydag/dag.py
--rw-r--r--   0 runner    (1001) docker     (121)    19079 2022-07-06 14:47:00.000000 historydag-1.0.1/historydag/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 14:47:09.844558 historydag-1.0.1/historydag.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4353 2022-07-06 14:47:09.000000 historydag-1.0.1/historydag.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      340 2022-07-06 14:47:09.000000 historydag-1.0.1/historydag.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-06 14:47:09.000000 historydag-1.0.1/historydag.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-07-06 14:47:09.000000 historydag-1.0.1/historydag.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-07-06 14:47:09.000000 historydag-1.0.1/historydag.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      313 2022-07-06 14:47:09.848558 historydag-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      800 2022-07-06 14:47:00.000000 historydag-1.0.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    80049 2022-07-06 14:47:00.000000 historydag-1.0.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:46:24.691183 historydag-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-06-08 18:46:12.000000 historydag-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-08 18:46:12.000000 historydag-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-06-08 18:46:24.691183 historydag-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-06-08 18:46:12.000000 historydag-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:46:24.691183 historydag-1.1.0/historydag/
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-08 18:46:12.000000 historydag-1.1.0/historydag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-08 18:46:24.695184 historydag-1.1.0/historydag/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-06-08 18:46:12.000000 historydag-1.1.0/historydag/beast_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11550 2023-06-08 18:46:12.000000 historydag-1.1.0/historydag/compact_genome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-08 18:46:12.000000 historydag-1.1.0/historydag/counterops.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144389 2023-06-08 18:46:12.000000 historydag-1.1.0/historydag/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19346 2023-06-08 18:46:12.000000 historydag-1.1.0/historydag/dag_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-06-08 18:46:12.000000 historydag-1.1.0/historydag/dag_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-06-08 18:46:12.000000 historydag-1.1.0/historydag/likelihoods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19220 2023-06-08 18:46:12.000000 historydag-1.1.0/historydag/mutation_annotated_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25401 2023-06-08 18:46:12.000000 historydag-1.1.0/historydag/parsimony.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30940 2023-06-08 18:46:12.000000 historydag-1.1.0/historydag/parsimony_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-06-08 18:46:12.000000 historydag-1.1.0/historydag/sankoff_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-06-08 18:46:12.000000 historydag-1.1.0/historydag/sequence_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33461 2023-06-08 18:46:12.000000 historydag-1.1.0/historydag/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:46:24.687183 historydag-1.1.0/historydag.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-06-08 18:46:24.000000 historydag-1.1.0/historydag.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-08 18:46:24.000000 historydag-1.1.0/historydag.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 18:46:24.000000 historydag-1.1.0/historydag.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-08 18:46:24.000000 historydag-1.1.0/historydag.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-08 18:46:24.000000 historydag-1.1.0/historydag.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-08 18:46:24.691183 historydag-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-08 18:46:12.000000 historydag-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:46:24.691183 historydag-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-06-08 18:46:12.000000 historydag-1.1.0/tests/test_collapse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-06-08 18:46:12.000000 historydag-1.1.0/tests/test_compact_genome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-06-08 18:46:12.000000 historydag-1.1.0/tests/test_dag_sankoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8614 2023-06-08 18:46:12.000000 historydag-1.1.0/tests/test_disambiguate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-06-08 18:46:12.000000 historydag-1.1.0/tests/test_edgeset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30552 2023-06-08 18:46:12.000000 historydag-1.1.0/tests/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-06-08 18:46:12.000000 historydag-1.1.0/tests/test_historydag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-08 18:46:12.000000 historydag-1.1.0/tests/test_mutation_annotated_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-08 18:46:12.000000 historydag-1.1.0/tests/test_node_insert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-08 18:46:12.000000 historydag-1.1.0/tests/test_subclass_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-06-08 18:46:12.000000 historydag-1.1.0/tests/test_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-08 18:46:12.000000 historydag-1.1.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-06-08 18:46:12.000000 historydag-1.1.0/versioneer.py
```

### Comparing `historydag-1.0.1/LICENSE` & `historydag-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `historydag-1.0.1/PKG-INFO` & `historydag-1.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: historydag
-Version: 1.0.1
+Version: 1.1.0
 Summary: Basic history DAG implementation
 Home-page: https://matsengrp.github.io/historydag
 Author: Will Dumm
 Author-email: wdumm88@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
@@ -18,38 +18,48 @@
 compactly expresses a collection of internally labeled trees which share
 a common set of leaf labels.
 
 ## Getting Started
 
 HistoryDAG is on PyPI! Install with `pip install historydag`.
 
-Alternatively, once you've cloned the repo, `pip install -e historydag` should be enough to
-get set up.
+Alternatively, clone the repo and perform `pip install -e historydag`.
 
-There is sample data in `sample_data/`. For example:
+The most common input for DAG construction is collections of
+[ete3](http://etetoolkit.org/) phylogenetic trees with full sequences at
+internal nodes stored in the `sequence` attribute. There is sample data like
+this in `sample_data/`. For example:
 
 ```python
 import historydag as hdag
 import pickle
 
 with open('sample_data/toy_trees.p', 'rb') as fh:
-	ete_trees = pickle.load(fh)
+    ete_trees = pickle.load(fh)
 
+# Build the DAG, specifying to only use the `sequence` attribute for node
+# labels (in general, one could use other attributes as well).
 dag = hdag.history_dag_from_etes(ete_trees, ['sequence'])
-dag.count_trees()  # 1041
+dag.count_histories()  # 1041
 
-dag.add_all_allowed_edges()
-dag.count_trees()  # 3431531
+# "Complete" the DAG, adding all allowable edges.
+dag.make_complete()
+dag.count_histories()  # 3431531
 
-dag.hamming_parsimony_count()  # Shows counts of trees of different parsimony scores
+# Show counts of trees with various parsimony scores.
+dag.hamming_parsimony_count()
+
+# "Trim" the DAG to make it only display minimum-weight trees.
 dag.trim_optimal_weight()
 # With default args, same as hamming_parsimony_count
 dag.weight_count()  # Counter({75: 45983})
 
+# "Collapse" the DAG, contracting zero-weight edges.
 dag.convert_to_collapsed()
+
 dag.weight_count()  # Counter({75: 1208})
 dag.count_topologies()  # 1054 unique topologies, ignoring internal labels
 
 # To count parsimony score and the number of unique nodes in each tree jointly:
 node_count_funcs = hdag.utils.AddFuncDict(
     {
         "start_func": lambda n: 0,
@@ -60,39 +70,38 @@
 )
 dag.weight_count(**(node_count_funcs + hdag.utils.hamming_distance_countfuncs))
 # Counter({(50, 75): 444, (51, 75): 328, (49, 75): 270, (52, 75): 94, (48, 75): 68, (53, 75): 4})
 
 # To trim to only the trees with 48 unique node labels:
 dag.trim_optimal_weight(**node_count_funcs, optimal_func=min)
 
-# Sample a tree from the dag and make it an ete tree
+# Sample a tree from the dag and make it an ete tree.
 t = dag.sample().to_ete()
 
 # the history DAG also supports indexing and iterating:
 t = dag[0].to_ete()
 trees = [tree for tree in dag]
 
 # Another method for fetching all trees in the dag is provided, but the order
 # will not match index order:
-scrambled_trees = list(dag.get_trees())
-
+scrambled_trees = list(dag.get_histories())
 
-# Union is implemented as dag merging, including with sequences of dags
+# Union is implemented as dag merging, including with sequences of dags.
 newdag = dag[0] | dag[1]
 newdag = dag[0] | (dag[i] for i in range(3,5))
 ```
 
 ### Highlights
 * History DAGs can be created with top-level functions like
     * `from_newick`
     * `from_ete`
     * `history_dag_from_newicks`
     * `history_dag_from_etes`
 * Trees can be extracted from the history DAG with methods like
-    * `HistoryDag.get_trees`
+    * `HistoryDag.get_histories`
     * `HistoryDag.sample`
     * `HistoryDag.to_ete`
     * `HistoryDag.to_newick` and `HistoryDag.to_newicks`
 * Simple history DAGs can be inspected with `HistoryDag.to_graphviz`
 * The DAG can be trimmed according to arbitrary tree weight functions. Use
     `HistoryDag.trim_optimal_weight`.
 * Disambiguation of sparse ambiguous labels can be done efficiently, but
```

### Comparing `historydag-1.0.1/README.md` & `historydag-1.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -4,38 +4,48 @@
 compactly expresses a collection of internally labeled trees which share
 a common set of leaf labels.
 
 ## Getting Started
 
 HistoryDAG is on PyPI! Install with `pip install historydag`.
 
-Alternatively, once you've cloned the repo, `pip install -e historydag` should be enough to
-get set up.
+Alternatively, clone the repo and perform `pip install -e historydag`.
 
-There is sample data in `sample_data/`. For example:
+The most common input for DAG construction is collections of
+[ete3](http://etetoolkit.org/) phylogenetic trees with full sequences at
+internal nodes stored in the `sequence` attribute. There is sample data like
+this in `sample_data/`. For example:
 
 ```python
 import historydag as hdag
 import pickle
 
 with open('sample_data/toy_trees.p', 'rb') as fh:
-	ete_trees = pickle.load(fh)
+    ete_trees = pickle.load(fh)
 
+# Build the DAG, specifying to only use the `sequence` attribute for node
+# labels (in general, one could use other attributes as well).
 dag = hdag.history_dag_from_etes(ete_trees, ['sequence'])
-dag.count_trees()  # 1041
+dag.count_histories()  # 1041
 
-dag.add_all_allowed_edges()
-dag.count_trees()  # 3431531
+# "Complete" the DAG, adding all allowable edges.
+dag.make_complete()
+dag.count_histories()  # 3431531
 
-dag.hamming_parsimony_count()  # Shows counts of trees of different parsimony scores
+# Show counts of trees with various parsimony scores.
+dag.hamming_parsimony_count()
+
+# "Trim" the DAG to make it only display minimum-weight trees.
 dag.trim_optimal_weight()
 # With default args, same as hamming_parsimony_count
 dag.weight_count()  # Counter({75: 45983})
 
+# "Collapse" the DAG, contracting zero-weight edges.
 dag.convert_to_collapsed()
+
 dag.weight_count()  # Counter({75: 1208})
 dag.count_topologies()  # 1054 unique topologies, ignoring internal labels
 
 # To count parsimony score and the number of unique nodes in each tree jointly:
 node_count_funcs = hdag.utils.AddFuncDict(
     {
         "start_func": lambda n: 0,
@@ -46,39 +56,38 @@
 )
 dag.weight_count(**(node_count_funcs + hdag.utils.hamming_distance_countfuncs))
 # Counter({(50, 75): 444, (51, 75): 328, (49, 75): 270, (52, 75): 94, (48, 75): 68, (53, 75): 4})
 
 # To trim to only the trees with 48 unique node labels:
 dag.trim_optimal_weight(**node_count_funcs, optimal_func=min)
 
-# Sample a tree from the dag and make it an ete tree
+# Sample a tree from the dag and make it an ete tree.
 t = dag.sample().to_ete()
 
 # the history DAG also supports indexing and iterating:
 t = dag[0].to_ete()
 trees = [tree for tree in dag]
 
 # Another method for fetching all trees in the dag is provided, but the order
 # will not match index order:
-scrambled_trees = list(dag.get_trees())
-
+scrambled_trees = list(dag.get_histories())
 
-# Union is implemented as dag merging, including with sequences of dags
+# Union is implemented as dag merging, including with sequences of dags.
 newdag = dag[0] | dag[1]
 newdag = dag[0] | (dag[i] for i in range(3,5))
 ```
 
 ### Highlights
 * History DAGs can be created with top-level functions like
     * `from_newick`
     * `from_ete`
     * `history_dag_from_newicks`
     * `history_dag_from_etes`
 * Trees can be extracted from the history DAG with methods like
-    * `HistoryDag.get_trees`
+    * `HistoryDag.get_histories`
     * `HistoryDag.sample`
     * `HistoryDag.to_ete`
     * `HistoryDag.to_newick` and `HistoryDag.to_newicks`
 * Simple history DAGs can be inspected with `HistoryDag.to_graphviz`
 * The DAG can be trimmed according to arbitrary tree weight functions. Use
     `HistoryDag.trim_optimal_weight`.
 * Disambiguation of sparse ambiguous labels can be done efficiently, but
```

### Comparing `historydag-1.0.1/historydag/counterops.py` & `historydag-1.1.0/historydag/counterops.py`

 * *Files identical despite different names*

### Comparing `historydag-1.0.1/historydag/utils.py` & `historydag-1.1.0/historydag/mutation_annotated_dag.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,593 +1,516 @@
-"""Utility functions and classes for working with HistoryDag objects."""
+"""This module allows the loading and manipulation of Larch mutation annotated
+DAG protobuf files.
 
-import ete3
-from Bio.Data.IUPACData import ambiguous_dna_values
-from collections import Counter
-from functools import wraps
-from collections import UserDict
-from decimal import Decimal
-from typing import (
-    List,
-    Any,
-    TypeVar,
-    Callable,
-    Union,
-    Iterable,
-    Generator,
-    Tuple,
-    NamedTuple,
-    Optional,
+The resulting history DAG contains labels with 'compact genomes', and a
+'refseq' attribute describing a reference sequence and set of mutations
+relative to the reference.
+"""
+
+import functools
+from frozendict import frozendict
+from historydag.dag import HistoryDag, HistoryDagNode, UANode, EdgeSet
+import historydag.utils
+from historydag.compact_genome import (
+    CompactGenome,
+    compact_genome_from_sequence,
+    cg_diff,
 )
-from typing import TYPE_CHECKING
-
-if TYPE_CHECKING:
-    from historydag.dag import HistoryDagNode
-
-Weight = Any
-Label = Union[NamedTuple, "UALabel"]
-F = TypeVar("F", bound=Callable[..., Any])
-
-
-class UALabel(str):
-    _fields: Tuple = tuple()
-
-    def __new__(cls):
-        return super(UALabel, cls).__new__(cls, "UA_Node")
-
-    def __eq__(self, other):
-        return isinstance(other, UALabel)
-
-    def __hash__(self):
-        return hash("UA_Node")
-
-    def __iter__(self):
-        raise RuntimeError("Attempted to iterate from dag root UALabel")
-
-    def _asdict(self):
-        raise RuntimeError("Attempted to iterate from dag root UALabel")
-
-
-bases = "AGCT-"
-ambiguous_dna_values.update({"?": bases, "-": "-"})
-
-
-# ######## Decorators ########
-def access_nodefield_default(fieldname: str, default: Any) -> Any:
-    """A decorator for accessing label fields on a HistoryDagNode. Converts a
-    function taking some label field's values as positional arguments, to a
-    function taking HistoryDagNodes as positional arguments.
-
-    Args:
-        fieldname: The name of the label field whose value the function takes as arguments
-        default: A value that should be returned if one of the arguments is the DAG UA node.
-
-    For example, instead of
-    `lambda n1, n2: default if n1.is_root() or n2.is_root() else func(n1.label.fieldname, n2.label.fieldname)`,
-    this wrapper allows one to write `access_nodefield_default(fieldname, default)(func)`.
-    """
-
-    def decorator(func):
-        @ignore_uanode(default)
-        @access_field("label")
-        @access_field(fieldname)
-        @wraps(func)
-        def wrapper(*args: Label, **kwargs: Any) -> Weight:
-            return func(*args, **kwargs)
-
-        return wrapper
-
-    return decorator
-
-
-def access_field(fieldname: str) -> Callable[[F], F]:
-    """A decorator for conveniently accessing a field in a label.
-
-    To be used instead of something like `lambda l1, l2:
-    func(l1.fieldname, l2.fieldname)`. Instead just write
-    `access_field(fieldname)(func)`. Supports arbitrarily many
-    positional arguments, which are all expected to be labels
-    (namedtuples) with field `fieldname`.
-    """
-
-    def decorator(func: F):
-        @wraps(func)
-        def wrapper(*args: Label, **kwargs: Any) -> Any:
-            newargs = [getattr(label, fieldname) for label in args]
-            return func(*newargs, **kwargs)
-
-        return wrapper
-
-    return decorator
-
-
-def ignore_uanode(default: Any) -> Callable[[F], F]:
-    """A decorator to return a default value if any argument is a UANode.
-
-    For instance, to allow distance between two nodes to be zero if one
-    is UANode
-    """
-
-    def decorator(func):
-        @wraps(func)
-        def wrapper(*args: "HistoryDagNode", **kwargs: Any):
-            for node in args:
-                if node.is_root():
-                    return default
-            else:
-                return func(*args, **kwargs)
-
-        return wrapper
-
-    return decorator
-
-
-def explode_label(labelfield: str):
-    """A decorator to make it easier to expand a Label by a certain field.
-
-    Args:
-        labelfield: the name of the field whose contents the wrapped function is expected to
-            explode
-
-    Returns:
-        A decorator which converts a function which explodes a field value, into a function
-        which explodes the whole label at that field.
-    """
-
-    def decorator(
-        func: Callable[[Any], Iterable[Any]]
-    ) -> Callable[[Label], Iterable[Label]]:
-        @wraps(func)
-        def wrapfunc(label, *args, **kwargs):
-            Label = type(label)
-            d = label._asdict()
-            for newval in func(d[labelfield], *args, **kwargs):
-                d[labelfield] = newval
-                yield Label(**d)
-
-        return wrapfunc
-
-    return decorator
-
-
-# ######## Distances and comparisons... ########
-
-
-def hamming_distance(s1: str, s2: str) -> int:
-    """The sitewise sum of base differences between s1 and s2."""
-    if len(s1) != len(s2):
-        raise ValueError("Sequences must have the same length!")
-    return sum(x != y for x, y in zip(s1, s2))
-
-
-@access_nodefield_default("sequence", 0)
-def wrapped_hamming_distance(s1, s2) -> int:
-    """The sitewise sum of base differences between sequence field contents of
-    two nodes.
-
-    Takes two HistoryDagNodes as arguments.
-
-    If l1 or l2 is a UANode, returns 0.
-    """
-    return hamming_distance(s1, s2)
-
-
-def is_ambiguous(sequence: str) -> bool:
-    """Returns whether the provided sequence contains IUPAC nucleotide
-    ambiguity codes."""
-    return any(code not in bases for code in sequence)
-
-
-def cartesian_product(
-    optionlist: List[Callable[[], Iterable]], accum=tuple()
-) -> Generator[Tuple, None, None]:
-    """The cartesian product of iterables in a list.
-
-    Takes a list of functions which each return a fresh generator on
-    options at that site, and returns a generator yielding tuples, which
-    are elements of the cartesian product of the passed generators'
-    contents.
-    """
-    if optionlist:
-        for term in optionlist[0]():
-            yield from cartesian_product(optionlist[1:], accum=(accum + (term,)))
-    else:
-        yield accum
-
-
-@explode_label("sequence")
-def sequence_resolutions(sequence: str) -> Generator[str, None, None]:
-    """Iterates through possible disambiguations of sequence, recursively.
-
-    Recursion-depth-limited by number of ambiguity codes in sequence,
-    not sequence length.
-    """
-
-    def _sequence_resolutions(sequence, _accum=""):
-        if sequence:
-            for index, base in enumerate(sequence):
-                if base in bases:
-                    _accum += base
-                else:
-                    for newbase in ambiguous_dna_values[base]:
-                        yield from _sequence_resolutions(
-                            sequence[index + 1 :], _accum=(_accum + newbase)
-                        )
-                    return
-        yield _accum
-
-    return _sequence_resolutions(sequence)
-
-
-@access_field("sequence")
-def sequence_resolutions_count(sequence: str) -> int:
-    """Count the number of possible sequence resolutions Equivalent to the
-    length of the list returned by :meth:`sequence_resolutions`."""
-    base_options = [
-        len(ambiguous_dna_values[base])
-        for base in sequence
-        if base in ambiguous_dna_values
-    ]
-    return prod(base_options)
-
+from historydag.parsimony_utils import (
+    compact_genome_hamming_distance_countfuncs,
+    leaf_ambiguous_compact_genome_hamming_distance_countfuncs,
+)
+import historydag.dag_pb2 as dpb
+import json
+from typing import NamedTuple
 
-def hist(c: Counter, samples: int = 1):
-    """Pretty prints a counter Normalizing counts using the number of samples,
-    passed as the argument `samples`."""
-    ls = list(c.items())
-    ls.sort()
-    print("Weight\t| Frequency\n------------------")
-    for weight, freq in ls:
-        print(f"{weight}  \t| {freq if samples==1 else freq/samples}")
 
+_pb_nuc_lookup = {0: "A", 1: "C", 2: "G", 3: "T"}
+_pb_nuc_codes = {nuc: code for code, nuc in _pb_nuc_lookup.items()}
 
-def is_collapsed(tree: ete3.TreeNode) -> bool:
-    """Return whether the provided tree is collapsed.
 
-    Collapsed means that any edge whose target is not a leaf node
-    connects nodes with different sequences.
-    """
-    return not any(
-        node.sequence == node.up.sequence and not node.is_leaf()
-        for node in tree.iter_descendants()
+def _pb_mut_to_str(mut):
+    """Unpack protobuf-encoded mutation into 1-indexed mutations string."""
+    return (
+        _pb_nuc_lookup[mut.par_nuc] + str(mut.position) + _pb_nuc_lookup[mut.mut_nuc[0]]
     )
 
 
-def collapse_adjacent_sequences(tree: ete3.TreeNode) -> ete3.TreeNode:
-    """Collapse nonleaf nodes that have the same sequence."""
-    # Need to keep doing this until the tree fully collapsed. See gctree for this!
-    tree = tree.copy()
-    to_delete = []
-    for node in tree.get_descendants():
-        # This must stay invariably hamming distance, since it's measuring equality of strings
-        if (
-            not node.is_leaf()
-            and hamming_distance(node.up.sequence, node.sequence) == 0
-        ):
-            to_delete.append(node)
-    for node in to_delete:
-        node.delete()
-    return tree
-
-
-class AddFuncDict(UserDict):
-    """Container for function keyword arguments to
-    :meth:`historydag.HistoryDag.weight_count`. This is primarily useful
-    because it allows instances to be added. Passing the result to
-    `weight_count` as keyword arguments counts the weights jointly. A
-    :class:`historydag.utils.AddFuncDict` which may be passed as keyword
-    arguments to :meth:`historydag.HistoryDag.weight_count`,
-    :meth:`historydag.HistoryDag.trim_optimal_weight`, or
-    :meth:`historydag.HistoryDag.optimal_weight_annotate` methods to trim or
-    annotate a :meth:`historydag.HistoryDag` according to the weight that the
-    contained functions implement.
-
-    For example, `dag.weight_count(**(utils.hamming_distance_countfuncs + make_newickcountfuncs()))`
-    would return a Counter object in which the weights are tuples containing hamming parsimony and newickstrings.
-
-    Args:
-        initialdata: A dictionary containing functions keyed by "start_func", "edge_weight_func", and
-            "accum_func". "start_func" specifies weight assigned to leaf HistoryDagNodes.
-            "edge_weight_func" specifies weight assigned to an edge between two HistoryDagNodes, with the
-            first argument the parent node, and the second argument the child node.
-            "accum_func" specifies how to 'add' a list of weights. See :meth:`historydag.HistoryDag.weight_count`
-            for more details.
-        name: A string containing a name for the weight to be counted. If a tuple of weights will be returned,
-            use ``names`` instead.
-        names: A tuple of strings containing names for the weights to be counted, if a tuple of weights will
-            be returned by passed functions. If only a single weight will be returned, use ``name`` instead.
-    """
-
-    requiredkeys = {"start_func", "edge_weight_func", "accum_func"}
-
-    def __init__(self, initialdata, name: str = None, names: Tuple[str] = None):
-        self.name: Optional[str]
-        self.names: Tuple[str]
-        if name is not None and names is not None:
-            raise ValueError(
-                "Pass a value to either keyword argument 'name' or 'names'."
-            )
-        elif name is None and names is None:
-            self.name = "unknown weight"
-            self.names = (self.name,)
-        elif name is not None:
-            self.name = name
-            self.names = (self.name,)
-        elif names is not None:
-            self.names = names
-            self.name = None
-        if not set(initialdata.keys()) == self.requiredkeys:
-            raise ValueError(
-                "Must provide functions named " + ", ".join(self.requiredkeys)
+class HDagJSONEncoder(json.JSONEncoder):
+    def default(self, obj):
+        if isinstance(obj, CompactGenome):
+            return dict(obj.mutations)
+        elif isinstance(obj, frozendict):
+            return dict(obj)
+        elif isinstance(obj, frozenset):
+            return list(obj)
+        return json.JSONEncoder.default(self, obj)
+
+
+class CGHistoryDag(HistoryDag):
+    """A HistoryDag subclass with node labels containing CompactGenome objects.
+
+    The constructor for this class requires that each node label contain
+    a 'compact_genome' field, which is expected to hold a
+    :class:`compact_genome.CompactGenome` object.
+
+    A HistoryDag containing 'sequence' node label fields may be
+    automatically converted to this subclass by calling the class method
+    :meth:`CGHistoryDag.from_dag`, providing the HistoryDag object to be
+    converted, and the reference sequence to the keyword argument
+    'reference'.
+
+    This subclass provides specialized methods for interfacing with
+    Larch's MADAG protobuf format
+    """
+
+    _required_label_fields = {
+        "compact_genome": [
+            (
+                ("sequence",),
+                lambda n, reference, **kwargs: compact_genome_from_sequence(
+                    n.label.sequence, reference, **kwargs
+                ),
             )
-        super().__init__(initialdata)
+        ]
+    }
 
-    def __add__(self, other) -> "AddFuncDict":
-        fdict1 = self._convert_to_tupleargs()
-        fdict2 = other._convert_to_tupleargs()
-        n = len(fdict1.names)
-
-        def newaccumfunc(weightlist):
-            return fdict1["accum_func"](
-                [weight[0:n] for weight in weightlist]
-            ) + fdict2["accum_func"]([weight[n:] for weight in weightlist])
-
-        def addfuncs(func1, func2):
-            def newfunc(*args):
-                return func1(*args) + func2(*args)
-
-            return newfunc
-
-        return AddFuncDict(
-            {
-                "start_func": addfuncs(fdict1["start_func"], fdict2["start_func"]),
-                "edge_weight_func": addfuncs(
-                    fdict1["edge_weight_func"], fdict2["edge_weight_func"]
-                ),
-                "accum_func": newaccumfunc,
-            },
-            names=fdict1.names + fdict2.names,
+    _default_args = frozendict(compact_genome_hamming_distance_countfuncs) | {
+        "start_func": (lambda n: 0),
+        "optimal_func": min,
+    }
+    # #### Overridden Methods ####
+
+    def weight_counts_with_ambiguities(self, *args, **kwargs):
+        raise NotImplementedError(
+            "This method is only implemented for DAGs with node labels containing sequences."
         )
 
-    def _convert_to_tupleargs(self):
-        if self.name is not None:
-
-            def node_to_weight_decorator(func):
-                @wraps(func)
-                def wrapper(*args):
-                    return (func(*args),)
-
-                return wrapper
-
-            def list_of_weights_to_weight_decorator(func):
-                @wraps(func)
-                def wrapper(weighttuplelist: List[Weight]):
-                    return (func([wt[0] for wt in weighttuplelist]),)
+    def summary(self):
+        HistoryDag.summary(self)
+        min_pars, max_pars = self.weight_range_annotate(
+            **compact_genome_hamming_distance_countfuncs
+        )
+        print(f"Parsimony score range {min_pars} to {max_pars}")
 
-                return wrapper
+    def hamming_parsimony_count(self):
+        """See :meth:`historydag.sequence_dag.SequenceHistoryDag.hamming_parsim
+        ony_count`"""
+        return self.weight_count(**compact_genome_hamming_distance_countfuncs)
+
+    # #### CGHistoryDag-Specific Methods ####
+
+    def to_protobuf(self, leaf_data_func=None):
+        """Convert a DAG with compact genome data on each node, to a MAD
+        protobuf with mutation information on edges.
+
+        Args:
+            dag: the history DAG to be converted
+            leaf_data_func: a function taking a DAG node and returning a string to store
+                in the protobuf node_name field `condensed_leaves` of leaf nodes
+        """
+
+        refseq = next(self.preorder(skip_ua_node=True)).label.compact_genome.reference
+        empty_cg = CompactGenome(dict(), refseq)
+
+        def mut_func(pnode, cnode):
+            if pnode.is_ua_node():
+                parent_seq = empty_cg
+            else:
+                parent_seq = pnode.label.compact_genome
+            return cg_diff(parent_seq, child.label.compact_genome)
 
-            return AddFuncDict(
-                {
-                    "start_func": node_to_weight_decorator(self["start_func"]),
-                    "edge_weight_func": node_to_weight_decorator(
-                        self["edge_weight_func"]
-                    ),
-                    "accum_func": list_of_weights_to_weight_decorator(
-                        self["accum_func"]
-                    ),
-                },
-                names=(self.name,),
+        def key_func(cladeitem):
+            clade, _ = cladeitem
+            return sorted(
+                sorted(idx for idx in label.compact_genome.mutations) for label in clade
             )
-        else:
-            return self
-
-
-hamming_distance_countfuncs = AddFuncDict(
-    {
-        "start_func": lambda n: 0,
-        "edge_weight_func": wrapped_hamming_distance,
-        "accum_func": sum,
-    },
-    name="HammingParsimony",
-)
-"""Provides functions to count hamming distance parsimony.
-For use with :meth:`historydag.HistoryDag.weight_count`."""
 
+        node_dict = {}
+        data = dpb.data()
+        for idx, node in enumerate(self.postorder()):
+            node_dict[node] = idx
+            node_name = data.node_names.add()
+            node_name.node_id = idx
+            if leaf_data_func is not None:
+                if node.is_leaf():
+                    node_name.condensed_leaves.append(leaf_data_func(node))
+
+        for node in self.postorder():
+            for cladeidx, (clade, edgeset) in enumerate(
+                sorted(node.clades.items(), key=key_func)
+            ):
+                for child in edgeset.targets:
+                    edge = data.edges.add()
+                    edge.parent_node = node_dict[node]
+                    edge.parent_clade = cladeidx
+                    edge.child_node = node_dict[child]
+                    for par_nuc, child_nuc, idx in mut_func(node, child):
+                        mut = edge.edge_mutations.add()
+                        mut.position = idx
+                        mut.par_nuc = _pb_nuc_codes[par_nuc.upper()]
+                        mut.mut_nuc.append(_pb_nuc_codes[child_nuc.upper()])
+        data.reference_seq = self.get_reference_sequence()
+        data.reference_id = (
+            self.attr["refseqid"] if "refseqid" in self.attr else "unknown_seqid"
+        )
+        return data
 
-def make_newickcountfuncs(
-    name_func=lambda n: "unnamed",
-    features=None,
-    feature_funcs={},
-    internal_labels=True,
-    collapse_leaves=False,
-):
-    """Provides functions to count newick strings. For use with
-    :meth:`historydag.HistoryDag.weight_count`.
-
-    Arguments are the same as for
-    :meth:`historydag.HistoryDag.to_newick`.
-    """
+    def to_protobuf_file(self, filename, leaf_data_func=None):
+        """Write this CGHistoryDag to a Mutation Annotated DAG protobuf for use
+        with Larch."""
+        data = self.to_protobuf(leaf_data_func=leaf_data_func)
+        with open(filename, "wb") as fh:
+            fh.write(data.SerializeToString())
+
+    def flatten(self, sort_compact_genomes=False):
+        """Return a dictionary containing four keys:
+
+        * `refseq` is a list containing the reference sequence id, and the reference sequence
+          (the implied sequence on the UA node)
+        * `compact_genome_list` is a list of compact genomes, where each compact genome is a
+          list of nested lists `[seq_idx, [old_base, new_base]]` where `seq_idx` is (1-indexed)
+          nucleotide sequence site. If sort_compact_genomes is True, compact genomes and `compact_genome_list` are sorted.
+        * `node_list` is a list of `[label_idx, clade_list]` pairs, where
+            * `label_idx` is the index of the node's compact genome in `compact_genome_list`, and
+            * `clade_list` is a list of lists of `compact_genome_list` indices, encoding sets of child clades.
+
+        * `edge_list` is a list of triples `[parent_idx, child_idx, clade_idx]`, where
+            * `parent_idx` is the index of the edge's parent node in `node_list`,
+            * `child_idx` is the index of the edge's child node in `node_list`, and
+            * `clade_idx` is the index of the clade in the parent node's `clade_list` from which this edge descends.
+        """
+        compact_genome_list = []
+        node_list = []
+        edge_list = []
+        node_indices = {}
+        cg_indices = {}
+
+        def get_child_clades(node):
+            return [
+                frozenset(cg_indices[label] for label in clade) for clade in node.clades
+            ]
+
+        def get_compact_genome(node):
+            if node.is_ua_node():
+                return []
+            else:
+                ret = [
+                    [idx, list(bases)]
+                    for idx, bases in node.label.compact_genome.mutations.items()
+                ]
+
+            if sort_compact_genomes:
+                ret.sort()
+            return ret
+
+        for node in self.postorder():
+            node_cg = get_compact_genome(node)
+            if node.label not in cg_indices:
+                cg_indices[node.label] = len(compact_genome_list)
+                compact_genome_list.append(node_cg)
+
+        if sort_compact_genomes:
+            cgindexlist = sorted(enumerate(compact_genome_list), key=lambda t: t[1])
+            compact_genome_list = [cg for _, cg in cgindexlist]
+            # the rearrangement is a bijection of indices
+            indexmap = {
+                oldidx: newidx for newidx, (oldidx, _) in enumerate(cgindexlist)
+            }
+            for key in cg_indices:
+                cg_indices[key] = indexmap[cg_indices[key]]
+
+        for node_idx, node in enumerate(self.postorder()):
+            node_indices[id(node)] = node_idx
+            node_list.append((cg_indices[node.label], get_child_clades(node)))
+            for clade_idx, (clade, eset) in enumerate(node.clades.items()):
+                for child in eset.targets:
+                    edge_list.append((node_idx, node_indices[id(child)], clade_idx))
 
-    def _newicksum(newicks):
-        # Filter out collapsed/deleted edges
-        snewicks = sorted(newicks)
-        if len(snewicks) == 2 and ";" in [newick[-1] for newick in snewicks if newick]:
-            # Then we are adding an edge above a complete tree
-            return "".join(
-                sorted(snewicks, key=lambda n: ";" == n[-1] if n else False)
-            )[:-1]
+        if "refseq" in self.attr:
+            refseqid = self.attr["refseq"]
         else:
-            # Then we're just accumulating options between clades
-            return "(" + ",".join(snewicks) + ")"
-
-    def _newickedgeweight(n1, n2):
-        if collapse_leaves and n2.is_leaf() and n1.label == n2.label:
-            return "COLLAPSED_LEAF;"
-        elif (
-            internal_labels
-            or n2.is_leaf()
-            or (collapse_leaves and frozenset({n2.label}) in n2.clades)
-        ):
-            return (
-                n2._newick_label(
-                    name_func=name_func, features=features, feature_funcs=feature_funcs
+            refseqid = "unknown_seqid"
+        return {
+            "refseq": (refseqid, self.get_reference_sequence()),
+            "compact_genomes": compact_genome_list,
+            "nodes": node_list,
+            "edges": edge_list,
+        }
+
+    def test_equal(self, other):
+        """Test whether two history DAGs are equal.
+
+        Compares sorted JSON representation.
+        """
+        flatdag1 = self.flatten()
+        flatdag2 = other.flatten()
+        cg_list1 = flatdag1["compact_genomes"]
+        cg_list2 = flatdag2["compact_genomes"]
+
+        def get_edge_set(flatdag):
+            edgelist = flatdag["edges"]
+            nodelist = flatdag["nodes"]
+
+            def convert_flatnode(flatnode):
+                label_idx, clade_list = flatnode
+                clades = frozenset(
+                    frozenset(label_idx_list) for label_idx_list in clade_list
                 )
-                + ";"
-            )
-        else:
-            return ";"
-
-    return AddFuncDict(
-        {
-            "start_func": lambda n: "",
-            "edge_weight_func": _newickedgeweight,
-            "accum_func": _newicksum,
-        },
-        name="NewickString",
-    )
+                return (label_idx, clades)
 
-
-def _cladetree_method(method):
-    """HistoryDagNode method decorator to ensure that the method is only run on
-    history DAGs which are clade trees."""
-
-    @wraps(method)
-    def wrapper(self, *args, **kwargs):
-        if not self.is_clade_tree():
-            raise ValueError(
-                "to_newick requires the history DAG to be a clade tree. "
-                "To extract newicks from a general DAG, see to_newicks"
+            nodelist = [convert_flatnode(node) for node in nodelist]
+            return frozenset(
+                (nodelist[p_idx], nodelist[c_idx]) for p_idx, c_idx, _ in edgelist
             )
-        else:
-            return method(self, *args, **kwargs)
-
-    return wrapper
-
-
-def prod(ls: list):
-    """Return product of elements of the input list.
-
-    if passed list is empty, returns 1.
-    """
-    n = len(ls)
-    if n > 0:
-        accum = ls[0]
-        if n > 1:
-            for item in ls[1:]:
-                accum *= item
-    else:
-        accum = 1
-    return accum
-
-
-# Unfortunately these can't be made with a class factory (just a bit too meta for Python)
-# short of doing something awful like https://hg.python.org/cpython/file/b14308524cff/Lib/collections/__init__.py#l232
-def _remstate(kwargs):
-    if "state" not in kwargs:
-        kwargs["state"] = None
-    intkwargs = kwargs.copy()
-    intkwargs.pop("state")
-    return intkwargs
-
-
-class IntState(int):
-    """A subclass of int, with arbitrary, mutable state.
-
-    State is provided to the constructor as the keyword argument
-    ``state``. All other arguments will be passed to ``int``
-    constructor. Instances should be functionally indistinguishable from
-    ``int``.
-    """
-
-    def __new__(cls, *args, **kwargs):
-        intkwargs = _remstate(kwargs)
-        return super(IntState, cls).__new__(cls, *args, **intkwargs)
-
-    def __init__(self, *args, **kwargs):
-        self.state = kwargs["state"]
 
-    def __copy__(self):
-        return IntState(int(self), state=self.state)
+        return cg_list1 == cg_list2 and get_edge_set(flatdag1) == get_edge_set(flatdag2)
 
-    def __getstate__(self):
-        return {"val": int(self), "state": self.state}
+    def get_reference_sequence(self):
+        """Return the reference sequence for this CGHistoryDag.
 
-    def __setstate__(self, statedict):
-        self.state = statedict["state"]
-
-
-class FloatState(float):
-    """A subclass of float, with arbitrary, mutable state.
-
-    State is provided to the constructor as the keyword argument
-    ``state``. All other arguments will be passed to ``float``
-    constructor. Instances should be functionally indistinguishable from
-    ``float``.
-    """
-
-    def __new__(cls, *args, **kwargs):
-        intkwargs = _remstate(kwargs)
-        return super(FloatState, cls).__new__(cls, *args, **intkwargs)
-
-    def __init__(self, *args, **kwargs):
-        self.state = kwargs["state"]
-
-    def __copy__(self):
-        return FloatState(float(self), state=self.state)
-
-    def __getstate__(self):
-        return {"val": float(self), "state": self.state}
-
-    def __setstate__(self, statedict):
-        self.state = statedict["state"]
-
-
-class DecimalState(Decimal):
-    """A subclass of ``decimal.Decimal``, with arbitrary, mutable state.
+        This is the sequence with respect to which all node label
+        CompactGenomes record mutations.
+        """
+        return next(self.preorder(skip_ua_node=True)).label.compact_genome.reference
+
+    def _check_valid(self, *args, **kwargs):
+        super()._check_valid(*args, **kwargs)
+        reference = self.get_reference_sequence()
+        for node in self.preorder(skip_ua_node=True):
+            if node.label.compact_genome.reference != reference:
+                raise ValueError(
+                    "Multiple compact genome reference sequences found in node label CompactGenomes."
+                )
 
-    State is provided to the constructor as the keyword argument
-    ``state``. All other arguments will be passed to ``Decimal``
-    constructor. Instances should be functionally indistinguishable from
-    ``Decimal``.
-    """
+    def to_json(self, sort_compact_genomes=False):
+        """Write this history DAG to a JSON object."""
+        return json.dumps(
+            self.flatten(sort_compact_genomes=sort_compact_genomes), cls=HDagJSONEncoder
+        )
 
-    def __new__(cls, *args, **kwargs):
-        intkwargs = _remstate(kwargs)
-        return super(DecimalState, cls).__new__(cls, *args, **intkwargs)
+    def to_json_file(self, filename, sort_compact_genomes=False):
+        """Write this history DAG to a JSON file."""
+        with open(filename, "w") as fh:
+            fh.write(self.to_json(sort_compact_genomes=sort_compact_genomes))
+
+
+class AmbiguousLeafCGHistoryDag(CGHistoryDag):
+    """A HistoryDag subclass with node labels containing compact genomes.
+
+    The constructor for this class requires that each node label contain
+    a 'compact_genome' field, which is expected to hold a
+    :class:`compact_genome.CompactGenome` object, which is expected to
+    hold an unambiguous sequence if the node is internal. The sequence
+    may contain ambiguities if the node is a leaf.
+
+    A HistoryDag containing 'sequence' node label fields may be
+    automatically converted to this subclass by calling the class method
+    :meth:`CGHistoryDag.from_dag`, providing the HistoryDag object to be
+    converted, and the reference sequence to the keyword argument
+    'reference'.
+    """
+
+    _default_args = frozendict(
+        leaf_ambiguous_compact_genome_hamming_distance_countfuncs
+    ) | {
+        "start_func": (lambda n: 0),
+        "optimal_func": min,
+    }
+
+    # #### Overridden Methods ####
+    def hamming_parsimony_count(self):
+        """See :meth:`historydag.sequence_dag.SequenceHistoryDag.hamming_parsim
+        ony_count`"""
+        return self.weight_count(
+            **leaf_ambiguous_compact_genome_hamming_distance_countfuncs
+        )
 
-    def __init__(self, *args, **kwargs):
-        self.state = kwargs["state"]
+    def summary(self):
+        HistoryDag.summary(self)
+        min_pars, max_pars = self.weight_range_annotate(
+            **leaf_ambiguous_compact_genome_hamming_distance_countfuncs
+        )
+        print(f"Parsimony score range {min_pars} to {max_pars}")
 
-    def __copy__(self):
-        return DecimalState(Decimal(self), state=self.state)
+    # #### End Overridden Methods ####
 
-    def __getstate__(self):
-        return {"val": Decimal(self), "state": self.state}
 
-    def __setstate__(self, statedict):
-        self.state = statedict["state"]
+def load_json_file(filename):
+    """Load a Mutation Annotated DAG stored in a JSON file and return a
+    CGHistoryDag."""
+    with open(filename, "r") as fh:
+        json_dict = json.load(fh)
+    return unflatten(json_dict)
+
+
+def unflatten(flat_dag):
+    """Takes a dictionary like that returned by flatten, and returns a
+    HistoryDag."""
+    refseqid, reference = flat_dag["refseq"]
+    compact_genome_list = [
+        CompactGenome({idx: tuple(bases) for idx, bases in flat_cg}, reference)
+        for flat_cg in flat_dag["compact_genomes"]
+    ]
+    node_list = flat_dag["nodes"]
+    edge_list = flat_dag["edges"]
+    Label = NamedTuple("Label", [("compact_genome", CompactGenome)])
+
+    def unpack_cladelabellists(cladelabelsetlist):
+        return [
+            frozenset(Label(compact_genome_list[cg_idx]) for cg_idx in idx_clade)
+            for idx_clade in cladelabelsetlist
+        ]
+
+    node_postorder = []
+    # a list of (node, [(clade, eset), ...]) tuples
+    for cg_idx, cladelabellists in node_list:
+        clade_eset_list = [
+            (clade, EdgeSet()) for clade in unpack_cladelabellists(cladelabellists)
+        ]
+        if len(clade_eset_list) == 1:
+            # This must be the UA node
+            label = historydag.utils.UALabel()
+        else:
+            label = Label(compact_genome_list[cg_idx])
+        try:
+            node = HistoryDagNode(label, dict(clade_eset_list), attr=None)
+        except ValueError:
+            node = UANode(clade_eset_list[0][1])
+        node_postorder.append((node, clade_eset_list))
+
+    # adjust UA node label
+    node_postorder[-1][0].label = historydag.utils.UALabel()
+
+    # Add edges
+    for parent_idx, child_idx, clade_idx in edge_list:
+        node_postorder[parent_idx][1][clade_idx][1].add_to_edgeset(
+            node_postorder[child_idx][0]
+        )
 
+    # UA node is last in postorder
+    dag = CGHistoryDag(node_postorder[-1][0])
+    dag.attr["refseq"] = refseqid
+    # This shouldn't be necessary, but appears to be
+    dag.recompute_parents()
+    return dag
+
+
+def load_MAD_protobuf(pbdata):
+    """Convert a MAD protobuf to a CGHistoryDag with compact genomes in the
+    `compact_genome` label attribute."""
+    # use HistoryDag.__setstate__ to make this happen
+    # all of a node's parent edges
+    reference = pbdata.reference_seq
+    parent_edges = {node.node_id: [] for node in pbdata.node_names}
+    # a list of list of a node's child edges
+    child_edges = {node.node_id: [] for node in pbdata.node_names}
+    for edge in pbdata.edges:
+        parent_edges[edge.child_node].append(edge)
+        child_edges[edge.parent_node].append(edge)
+
+    # now each node id is in parent_edges and child_edges as a key,
+    # fix the UA node's compact genome (could be done in function but this
+    # asserts only one node has no parent edges)
+    (ua_node_id,) = [
+        node_id for node_id, eset in parent_edges.items() if len(eset) == 0
+    ]
 
-class StrState(str):
-    """A subclass of string, with arbitrary, mutable state.
+    @functools.lru_cache(maxsize=None)
+    def get_node_compact_genome(node_id):
+        if node_id == ua_node_id:
+            return CompactGenome(frozendict(), reference)
+        else:
+            edge = parent_edges[node_id][0]
+            parent_seq = get_node_compact_genome(edge.parent_node)
+            str_mutations = tuple(_pb_mut_to_str(mut) for mut in edge.edge_mutations)
+            return parent_seq.apply_muts(str_mutations)
+
+    label_list = []
+    label_dict = {}
+
+    for node_record in pbdata.node_names:
+        cg = get_node_compact_genome(node_record.node_id)
+        if cg in label_dict:
+            cg_idx = label_dict[cg]
+        else:
+            cg_idx = len(label_list)
+            label_dict[cg] = cg_idx
+            label_list.append(cg)
+
+    # now build clade unions by dynamic programming:
+    @functools.lru_cache(maxsize=None)
+    def get_clade_union(node_id):
+        if len(child_edges[node_id]) == 0:
+            # it's a leaf node
+            return frozenset({label_dict[get_node_compact_genome(node_id)]})
+        else:
+            return frozenset(
+                {
+                    label
+                    for child_edge in child_edges[node_id]
+                    for label in get_clade_union(child_edge.child_node)
+                }
+            )
 
-    State is provided to the constructor as the keyword argument
-    ``state``. All other arguments will be passed to ``str``
-    constructor. Instances should be functionally indistinguishable from
-    ``str``.
-    """
+    def get_child_clades(node_id):
+        return tuple(
+            get_clade_union(child_edge.child_node)
+            for child_edge in child_edges[node_id]
+        )
+        # maybe we need this??
+        # return frozenset({get_clade_union(child_edge.child_node) for child_edge in child_edges[node_id]})
 
-    def __new__(cls, *args, **kwargs):
-        intkwargs = _remstate(kwargs)
-        return super(StrState, cls).__new__(cls, *args, **intkwargs)
+    # order node_ids in postordering
+    visited = set()
 
-    def __init__(self, *args, **kwargs):
-        self.state = kwargs["state"]
+    def traverse(node_id):
+        visited.add(node_id)
+        child_ids = [edge.child_node for edge in child_edges[node_id]]
+        if len(child_ids) > 0:
+            for child_id in child_ids:
+                if child_id not in visited:
+                    yield from traverse(child_id)
+        yield node_id
+
+    id_postorder = list(traverse(ua_node_id))
+    # Start building DAG data
+    node_index_d = {node_id: idx for idx, node_id in enumerate(id_postorder)}
+    node_list = [
+        (
+            label_dict[get_node_compact_genome(node_id)],
+            get_child_clades(node_id),
+            {"node_id": node_id},
+        )
+        for node_id in id_postorder
+    ]
 
-    def __copy__(self):
-        return StrState(str(self), state=self.state)
+    edge_list = [
+        (node_index_d[edge.parent_node], node_index_d[edge.child_node], 0, 1)
+        for edge in pbdata.edges
+    ]
+    # fix label list
+    label_list = [(item,) for item in label_list]
+    label_list.append(None)
+    ua_node = list(node_list[-1])
+    ua_node[0] = len(label_list) - 1
+    node_list[-1] = tuple(ua_node)
+    dag = HistoryDag(UANode(EdgeSet()))
+    dag.__setstate__(
+        {
+            "label_fields": ("compact_genome",),
+            "label_list": label_list,
+            "node_list": node_list,
+            "edge_list": edge_list,
+            "attr": {"refseqid": pbdata.reference_id},
+        }
+    )
+    return CGHistoryDag.from_history_dag(dag)
 
-    def __getstate__(self):
-        return {"val": str(self), "state": self.state}
 
-    def __setstate__(self, statedict):
-        self.state = statedict["state"]
+def load_MAD_protobuf_file(filename):
+    """Load a mutation annotated DAG protobuf file and return a
+    CGHistoryDag."""
+    with open(filename, "rb") as fh:
+        pb_data = dpb.data()
+        pb_data.ParseFromString(fh.read())
+    return load_MAD_protobuf(pb_data)
```

### Comparing `historydag-1.0.1/historydag.egg-info/PKG-INFO` & `historydag-1.1.0/historydag.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: historydag
-Version: 1.0.1
+Version: 1.1.0
 Summary: Basic history DAG implementation
 Home-page: https://matsengrp.github.io/historydag
 Author: Will Dumm
 Author-email: wdumm88@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
@@ -18,38 +18,48 @@
 compactly expresses a collection of internally labeled trees which share
 a common set of leaf labels.
 
 ## Getting Started
 
 HistoryDAG is on PyPI! Install with `pip install historydag`.
 
-Alternatively, once you've cloned the repo, `pip install -e historydag` should be enough to
-get set up.
+Alternatively, clone the repo and perform `pip install -e historydag`.
 
-There is sample data in `sample_data/`. For example:
+The most common input for DAG construction is collections of
+[ete3](http://etetoolkit.org/) phylogenetic trees with full sequences at
+internal nodes stored in the `sequence` attribute. There is sample data like
+this in `sample_data/`. For example:
 
 ```python
 import historydag as hdag
 import pickle
 
 with open('sample_data/toy_trees.p', 'rb') as fh:
-	ete_trees = pickle.load(fh)
+    ete_trees = pickle.load(fh)
 
+# Build the DAG, specifying to only use the `sequence` attribute for node
+# labels (in general, one could use other attributes as well).
 dag = hdag.history_dag_from_etes(ete_trees, ['sequence'])
-dag.count_trees()  # 1041
+dag.count_histories()  # 1041
 
-dag.add_all_allowed_edges()
-dag.count_trees()  # 3431531
+# "Complete" the DAG, adding all allowable edges.
+dag.make_complete()
+dag.count_histories()  # 3431531
 
-dag.hamming_parsimony_count()  # Shows counts of trees of different parsimony scores
+# Show counts of trees with various parsimony scores.
+dag.hamming_parsimony_count()
+
+# "Trim" the DAG to make it only display minimum-weight trees.
 dag.trim_optimal_weight()
 # With default args, same as hamming_parsimony_count
 dag.weight_count()  # Counter({75: 45983})
 
+# "Collapse" the DAG, contracting zero-weight edges.
 dag.convert_to_collapsed()
+
 dag.weight_count()  # Counter({75: 1208})
 dag.count_topologies()  # 1054 unique topologies, ignoring internal labels
 
 # To count parsimony score and the number of unique nodes in each tree jointly:
 node_count_funcs = hdag.utils.AddFuncDict(
     {
         "start_func": lambda n: 0,
@@ -60,39 +70,38 @@
 )
 dag.weight_count(**(node_count_funcs + hdag.utils.hamming_distance_countfuncs))
 # Counter({(50, 75): 444, (51, 75): 328, (49, 75): 270, (52, 75): 94, (48, 75): 68, (53, 75): 4})
 
 # To trim to only the trees with 48 unique node labels:
 dag.trim_optimal_weight(**node_count_funcs, optimal_func=min)
 
-# Sample a tree from the dag and make it an ete tree
+# Sample a tree from the dag and make it an ete tree.
 t = dag.sample().to_ete()
 
 # the history DAG also supports indexing and iterating:
 t = dag[0].to_ete()
 trees = [tree for tree in dag]
 
 # Another method for fetching all trees in the dag is provided, but the order
 # will not match index order:
-scrambled_trees = list(dag.get_trees())
-
+scrambled_trees = list(dag.get_histories())
 
-# Union is implemented as dag merging, including with sequences of dags
+# Union is implemented as dag merging, including with sequences of dags.
 newdag = dag[0] | dag[1]
 newdag = dag[0] | (dag[i] for i in range(3,5))
 ```
 
 ### Highlights
 * History DAGs can be created with top-level functions like
     * `from_newick`
     * `from_ete`
     * `history_dag_from_newicks`
     * `history_dag_from_etes`
 * Trees can be extracted from the history DAG with methods like
-    * `HistoryDag.get_trees`
+    * `HistoryDag.get_histories`
     * `HistoryDag.sample`
     * `HistoryDag.to_ete`
     * `HistoryDag.to_newick` and `HistoryDag.to_newicks`
 * Simple history DAGs can be inspected with `HistoryDag.to_graphviz`
 * The DAG can be trimmed according to arbitrary tree weight functions. Use
     `HistoryDag.trim_optimal_weight`.
 * Disambiguation of sparse ambiguous labels can be done efficiently, but
```

### Comparing `historydag-1.0.1/setup.py` & `historydag-1.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,9 +17,9 @@
     packages=["historydag"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License (GPL)",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.7",
-    install_requires=["six", "PyQt5", "ete3", "biopython", "graphviz"],
+    install_requires=["six", "PyQt5", "ete3", "biopython", "graphviz", "frozendict", "protobuf"],
 )
```

### Comparing `historydag-1.0.1/versioneer.py` & `historydag-1.1.0/versioneer.py`

 * *Files identical despite different names*

