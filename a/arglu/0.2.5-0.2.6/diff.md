# Comparing `tmp/arglu-0.2.5.tar.gz` & `tmp/arglu-0.2.6.tar.gz`

## Comparing `arglu-0.2.5.tar` & `arglu-0.2.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arglu-0.2.5/src/arglu/__init__.py
--rw-r--r--   0        0        0     3015 2020-02-02 00:00:00.000000 arglu-0.2.5/src/arglu/file_type_utils.py
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 arglu-0.2.5/src/arglu/graph_processing.py
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 arglu-0.2.5/src/arglu/mutable_tree.py
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 arglu-0.2.5/src/arglu/node.py
--rw-r--r--   0        0        0     8173 2020-02-02 00:00:00.000000 arglu-0.2.5/src/arglu/plot_argument_graphs.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 arglu-0.2.5/LICENSE
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 arglu-0.2.5/README.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 arglu-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 arglu-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arglu-0.2.6/src/arglu/__init__.py
+-rw-r--r--   0        0        0     3015 2020-02-02 00:00:00.000000 arglu-0.2.6/src/arglu/file_type_utils.py
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 arglu-0.2.6/src/arglu/graph_processing.py
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 arglu-0.2.6/src/arglu/mutable_tree.py
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 arglu-0.2.6/src/arglu/node.py
+-rw-r--r--   0        0        0     8213 2020-02-02 00:00:00.000000 arglu-0.2.6/src/arglu/plot_argument_graphs.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 arglu-0.2.6/LICENSE
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 arglu-0.2.6/README.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 arglu-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 arglu-0.2.6/PKG-INFO
```

### Comparing `arglu-0.2.5/src/arglu/file_type_utils.py` & `arglu-0.2.6/src/arglu/file_type_utils.py`

 * *Files identical despite different names*

### Comparing `arglu-0.2.5/src/arglu/graph_processing.py` & `arglu-0.2.6/src/arglu/graph_processing.py`

 * *Files identical despite different names*

### Comparing `arglu-0.2.5/src/arglu/mutable_tree.py` & `arglu-0.2.6/src/arglu/mutable_tree.py`

 * *Files identical despite different names*

### Comparing `arglu-0.2.5/src/arglu/node.py` & `arglu-0.2.6/src/arglu/node.py`

 * *Files identical despite different names*

### Comparing `arglu-0.2.5/src/arglu/plot_argument_graphs.py` & `arglu-0.2.6/src/arglu/plot_argument_graphs.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,14 +190,15 @@
         
     def draw_graph(self):
         
         G = self.graph
         self.positions = graphviz_layout(G, prog="dot")
 
         if self.colour_map:
+            import pdb; pdb.set_trace()
             node_colours = [self.colour_map[k] for k in G.nodes().keys()]
         else:
             node_colours = ["gray"] * len(self.positions)
 
         self.nodes = nx.draw_networkx_nodes(G, self.positions, node_color=node_colours)#, node_size=node_size)
         nx.draw_networkx_labels(G, self.positions)#, font_size=font_size)
         nx.draw_networkx_edges(G, self.positions), #edgelist=edge_pairs, arrows=True, arrowsize=arrowsize, arrowstyle=arrowstyle, alpha=1)
```

### Comparing `arglu-0.2.5/LICENSE` & `arglu-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `arglu-0.2.5/pyproject.toml` & `arglu-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "arglu"
-version = "0.2.5"
+version = "0.2.6"
 authors = [
   { name="Jonathan Clayton", email="jaclayton2@sheffield.ac.uk" },
 ]
 description = "Some utilities for Argument Mining"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `arglu-0.2.5/PKG-INFO` & `arglu-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arglu
-Version: 0.2.5
+Version: 0.2.6
 Summary: Some utilities for Argument Mining
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Jonathan Clayton <jaclayton2@sheffield.ac.uk>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

