# Comparing `tmp/xaddpy-0.1.8.tar.gz` & `tmp/xaddpy-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xaddpy-0.1.8.tar", last modified: Wed Jan 18 14:30:36 2023, max compression
+gzip compressed data, was "xaddpy-0.1.9.tar", last modified: Wed Jan 18 15:12:31 2023, max compression
```

## Comparing `xaddpy-0.1.8.tar` & `xaddpy-0.1.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 jihwan    (1000) jihwan    (1000)        0 2023-01-18 14:30:36.378249 xaddpy-0.1.8/
--rw-rw-r--   0 jihwan    (1000) jihwan    (1000)     1069 2022-08-27 01:07:34.000000 xaddpy-0.1.8/LICENSE
--rw-rw-r--   0 jihwan    (1000) jihwan    (1000)     7384 2023-01-18 14:30:36.378249 xaddpy-0.1.8/PKG-INFO
--rw-rw-r--   0 jihwan    (1000) jihwan    (1000)     5436 2023-01-18 14:09:19.000000 xaddpy-0.1.8/README.md
--rw-rw-r--   0 jihwan    (1000) jihwan    (1000)      721 2023-01-18 14:21:19.000000 xaddpy-0.1.8/pyproject.toml
--rw-rw-r--   0 jihwan    (1000) jihwan    (1000)       38 2023-01-18 14:30:36.378249 xaddpy-0.1.8/setup.cfg
--rw-rw-r--   0 jihwan    (1000) jihwan    (1000)      602 2023-01-18 14:21:43.000000 xaddpy-0.1.8/setup.py
-drwxrwxr-x   0 jihwan    (1000) jihwan    (1000)        0 2023-01-18 14:30:36.374249 xaddpy-0.1.8/xaddpy/
--rw-rw-r--   0 jihwan    (1000) jihwan    (1000)       90 2023-01-18 12:23:14.000000 xaddpy-0.1.8/xaddpy/__init__.py
-drwxrwxr-x   0 jihwan    (1000) jihwan    (1000)        0 2023-01-18 14:30:36.374249 xaddpy-0.1.8/xaddpy/utils/
--rw-rw-r--   0 jihwan    (1000) jihwan    (1000)       33 2023-01-18 12:23:14.000000 xaddpy-0.1.8/xaddpy/utils/__init__.py
--rw-rw-r--   0 jihwan    (1000) jihwan    (1000)     1222 2023-01-18 12:23:14.000000 xaddpy-0.1.8/xaddpy/utils/global_vars.py
--rw-rw-r--   0 jihwan    (1000) jihwan    (1000)     2690 2023-01-18 12:23:14.000000 xaddpy-0.1.8/xaddpy/utils/graph.py
--rw-rw-r--   0 jihwan    (1000) jihwan    (1000)     1162 2022-08-27 01:07:34.000000 xaddpy-0.1.8/xaddpy/utils/logger.py
--rw-rw-r--   0 jihwan    (1000) jihwan    (1000)     8584 2023-01-18 12:23:14.000000 xaddpy-0.1.8/xaddpy/utils/lp_util.py
--rw-rw-r--   0 jihwan    (1000) jihwan    (1000)     8730 2023-01-18 12:23:14.000000 xaddpy-0.1.8/xaddpy/utils/util.py
-drwxrwxr-x   0 jihwan    (1000) jihwan    (1000)        0 2023-01-18 14:30:36.378249 xaddpy-0.1.8/xaddpy/xadd/
--rw-rw-r--   0 jihwan    (1000) jihwan    (1000)       46 2023-01-18 12:23:14.000000 xaddpy-0.1.8/xaddpy/xadd/__init__.py
--rw-rw-r--   0 jihwan    (1000) jihwan    (1000)    11361 2023-01-18 13:56:53.000000 xaddpy-0.1.8/xaddpy/xadd/node.py
--rw-rw-r--   0 jihwan    (1000) jihwan    (1000)    17697 2023-01-18 12:23:14.000000 xaddpy-0.1.8/xaddpy/xadd/reduce_lp.py
--rw-rw-r--   0 jihwan    (1000) jihwan    (1000)    88437 2023-01-18 13:49:23.000000 xaddpy-0.1.8/xaddpy/xadd/xadd.py
--rw-rw-r--   0 jihwan    (1000) jihwan    (1000)     1652 2023-01-18 12:23:14.000000 xaddpy-0.1.8/xaddpy/xadd/xadd_parse_utils.py
-drwxrwxr-x   0 jihwan    (1000) jihwan    (1000)        0 2023-01-18 14:30:36.374249 xaddpy-0.1.8/xaddpy.egg-info/
--rw-rw-r--   0 jihwan    (1000) jihwan    (1000)     7384 2023-01-18 14:30:36.000000 xaddpy-0.1.8/xaddpy.egg-info/PKG-INFO
--rw-rw-r--   0 jihwan    (1000) jihwan    (1000)      473 2023-01-18 14:30:36.000000 xaddpy-0.1.8/xaddpy.egg-info/SOURCES.txt
--rw-rw-r--   0 jihwan    (1000) jihwan    (1000)        1 2023-01-18 14:30:36.000000 xaddpy-0.1.8/xaddpy.egg-info/dependency_links.txt
--rw-rw-r--   0 jihwan    (1000) jihwan    (1000)       24 2023-01-18 14:30:36.000000 xaddpy-0.1.8/xaddpy.egg-info/requires.txt
--rw-rw-r--   0 jihwan    (1000) jihwan    (1000)        7 2023-01-18 14:30:36.000000 xaddpy-0.1.8/xaddpy.egg-info/top_level.txt
+drwxrwxr-x   0 jihwan    (1000) jihwan    (1000)        0 2023-01-18 15:12:31.831854 xaddpy-0.1.9/
+-rw-rw-r--   0 jihwan    (1000) jihwan    (1000)     1069 2022-08-27 01:07:34.000000 xaddpy-0.1.9/LICENSE
+-rw-rw-r--   0 jihwan    (1000) jihwan    (1000)     7384 2023-01-18 15:12:31.831854 xaddpy-0.1.9/PKG-INFO
+-rw-rw-r--   0 jihwan    (1000) jihwan    (1000)     5436 2023-01-18 14:09:19.000000 xaddpy-0.1.9/README.md
+-rw-rw-r--   0 jihwan    (1000) jihwan    (1000)      721 2023-01-18 15:09:43.000000 xaddpy-0.1.9/pyproject.toml
+-rw-rw-r--   0 jihwan    (1000) jihwan    (1000)       38 2023-01-18 15:12:31.831854 xaddpy-0.1.9/setup.cfg
+-rw-rw-r--   0 jihwan    (1000) jihwan    (1000)      602 2023-01-18 15:09:53.000000 xaddpy-0.1.9/setup.py
+drwxrwxr-x   0 jihwan    (1000) jihwan    (1000)        0 2023-01-18 15:12:31.831854 xaddpy-0.1.9/xaddpy/
+-rw-rw-r--   0 jihwan    (1000) jihwan    (1000)       90 2023-01-18 12:23:14.000000 xaddpy-0.1.9/xaddpy/__init__.py
+drwxrwxr-x   0 jihwan    (1000) jihwan    (1000)        0 2023-01-18 15:12:31.831854 xaddpy-0.1.9/xaddpy/utils/
+-rw-rw-r--   0 jihwan    (1000) jihwan    (1000)       33 2023-01-18 12:23:14.000000 xaddpy-0.1.9/xaddpy/utils/__init__.py
+-rw-rw-r--   0 jihwan    (1000) jihwan    (1000)     1222 2023-01-18 12:23:14.000000 xaddpy-0.1.9/xaddpy/utils/global_vars.py
+-rw-rw-r--   0 jihwan    (1000) jihwan    (1000)     2690 2023-01-18 12:23:14.000000 xaddpy-0.1.9/xaddpy/utils/graph.py
+-rw-rw-r--   0 jihwan    (1000) jihwan    (1000)     1162 2022-08-27 01:07:34.000000 xaddpy-0.1.9/xaddpy/utils/logger.py
+-rw-rw-r--   0 jihwan    (1000) jihwan    (1000)     8584 2023-01-18 12:23:14.000000 xaddpy-0.1.9/xaddpy/utils/lp_util.py
+-rw-rw-r--   0 jihwan    (1000) jihwan    (1000)     8730 2023-01-18 12:23:14.000000 xaddpy-0.1.9/xaddpy/utils/util.py
+drwxrwxr-x   0 jihwan    (1000) jihwan    (1000)        0 2023-01-18 15:12:31.831854 xaddpy-0.1.9/xaddpy/xadd/
+-rw-rw-r--   0 jihwan    (1000) jihwan    (1000)       46 2023-01-18 12:23:14.000000 xaddpy-0.1.9/xaddpy/xadd/__init__.py
+-rw-rw-r--   0 jihwan    (1000) jihwan    (1000)    11612 2023-01-18 15:05:05.000000 xaddpy-0.1.9/xaddpy/xadd/node.py
+-rw-rw-r--   0 jihwan    (1000) jihwan    (1000)    17697 2023-01-18 12:23:14.000000 xaddpy-0.1.9/xaddpy/xadd/reduce_lp.py
+-rw-rw-r--   0 jihwan    (1000) jihwan    (1000)    88814 2023-01-18 15:00:20.000000 xaddpy-0.1.9/xaddpy/xadd/xadd.py
+-rw-rw-r--   0 jihwan    (1000) jihwan    (1000)     1652 2023-01-18 12:23:14.000000 xaddpy-0.1.9/xaddpy/xadd/xadd_parse_utils.py
+drwxrwxr-x   0 jihwan    (1000) jihwan    (1000)        0 2023-01-18 15:12:31.831854 xaddpy-0.1.9/xaddpy.egg-info/
+-rw-rw-r--   0 jihwan    (1000) jihwan    (1000)     7384 2023-01-18 15:12:31.000000 xaddpy-0.1.9/xaddpy.egg-info/PKG-INFO
+-rw-rw-r--   0 jihwan    (1000) jihwan    (1000)      473 2023-01-18 15:12:31.000000 xaddpy-0.1.9/xaddpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 jihwan    (1000) jihwan    (1000)        1 2023-01-18 15:12:31.000000 xaddpy-0.1.9/xaddpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 jihwan    (1000) jihwan    (1000)       24 2023-01-18 15:12:31.000000 xaddpy-0.1.9/xaddpy.egg-info/requires.txt
+-rw-rw-r--   0 jihwan    (1000) jihwan    (1000)        7 2023-01-18 15:12:31.000000 xaddpy-0.1.9/xaddpy.egg-info/top_level.txt
```

### Comparing `xaddpy-0.1.8/LICENSE` & `xaddpy-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `xaddpy-0.1.8/PKG-INFO` & `xaddpy-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: xaddpy
-Version: 0.1.8
+Version: 0.1.9
 Summary: XADD package in Python
 Home-page: https://github.com/jihwan-jeong/xaddpy
-Download-URL: https://github.com/jihwan-jeong/xaddpy/archive/refs/tags/0.1.8.tar.gz
+Download-URL: https://github.com/jihwan-jeong/xaddpy/archive/refs/tags/0.1.9.tar.gz
 Author: Jihwan Jeong
 Author-email: Jihwan Jeong <jiihwan.jeong@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 jihwan-jeong
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `xaddpy-0.1.8/README.md` & `xaddpy-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `xaddpy-0.1.8/pyproject.toml` & `xaddpy-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xaddpy"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="Jihwan Jeong", email="jiihwan.jeong@gmail.com" },
 ]
 license = {file = "LICENSE"}
 keywords  = ["xadd", "xadd python", "symbolic diagram"]
 description = "XADD package in Python"
 readme = "README.md"
```

### Comparing `xaddpy-0.1.8/setup.py` & `xaddpy-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='xaddpy',
     packages=find_packages(),
-    version='0.1.8',
+    version='0.1.9',
     license='MIT License',
     description='XADD package in Python',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Jihwan Jeong',
     author_email='jiihwan.jeong@gmail.com',
     url='https://github.com/jihwan-jeong/xaddpy',
-    download_url="https://github.com/jihwan-jeong/xaddpy/archive/refs/tags/0.1.8.tar.gz"
+    download_url="https://github.com/jihwan-jeong/xaddpy/archive/refs/tags/0.1.9.tar.gz"
 )
```

### Comparing `xaddpy-0.1.8/xaddpy/utils/global_vars.py` & `xaddpy-0.1.9/xaddpy/utils/global_vars.py`

 * *Files identical despite different names*

### Comparing `xaddpy-0.1.8/xaddpy/utils/graph.py` & `xaddpy-0.1.9/xaddpy/utils/graph.py`

 * *Files identical despite different names*

### Comparing `xaddpy-0.1.8/xaddpy/utils/logger.py` & `xaddpy-0.1.9/xaddpy/utils/logger.py`

 * *Files identical despite different names*

### Comparing `xaddpy-0.1.8/xaddpy/utils/lp_util.py` & `xaddpy-0.1.9/xaddpy/utils/lp_util.py`

 * *Files identical despite different names*

### Comparing `xaddpy-0.1.8/xaddpy/utils/util.py` & `xaddpy-0.1.9/xaddpy/utils/util.py`

 * *Files identical despite different names*

### Comparing `xaddpy-0.1.8/xaddpy/xadd/node.py` & `xaddpy-0.1.9/xaddpy/xadd/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,20 @@
+import warnings
 import sympy.core.relational as relational
 import sympy
 from sympy import oo
 import abc
 
-from xaddpy.utils.graph import Graph
+try:
+    from xaddpy.utils.graph import Graph
+except ImportError:
+    warnings.warn("[Module: xaddpy.xadd.node] Import error: pygraphviz not installed")
+    class Graph:
+        def __init__(self, *args, **kwargs):
+            pass
 
 
 class Node(metaclass=abc.ABCMeta):
     def __init__(self, context):
         self._context = context
         self._print_node_info = True
         self._is_leaf = False
@@ -299,52 +306,52 @@
 
     def __str__(self, level=0):
         ret = ""
         ret += f"( [{self._context._id_to_expr[self.dec]}]"
 
         # print node id
         if self._print_node_info:
-            ret += f" (dec, id): {self.dec}, {self._context._node_to_id.get(self)}"
+            ret += f" \t(dec, id): {self.dec}, {self._context._node_to_id.get(self)}"
 
         # Node level cache
         high = self._context._id_to_node.get(self._high, None)
         if high is not None:
-            ret += "\n" + "\t"*(level+1) + f" {high.__str__(level+1)} "
+            ret += "\n" + "\t"*(level+1) + f"{high.__str__(level+1)} "
         else:
             ret += "h:[None] "
 
         low = self._context._id_to_node.get(self._low, None)
         if low is not None:
-            ret += "\n" + "\t" * (level + 1) + f" {low.__str__(level + 1)} "
+            ret += "\n" + "\t" * (level + 1) + f"{low.__str__(level + 1)} "
         else:
             ret += "l:[None] "
-        ret += "\n) "
+        ret += "\n" + "\t" * level + ") "
         return ret
 
     def __repr__(self, level=0):
         ret = ""
         ret += f"( [{self._context._id_to_expr[self.dec]}]"
 
         # print node id
         if self._print_node_info:
-            ret += f" (dec, id): {self.dec}, {self._context._node_to_id.get(self)}"
+            ret += f" \t(dec, id): {self.dec}, {self._context._node_to_id.get(self)}"
 
         # Node level cache
         high = self._context._id_to_node.get(self._high, None)
         if high is not None:
-            ret += "\n" + "\t"*(level+1) + f" {high.__str__(level+1)} "
+            ret += "\n" + "\t"*(level+1) + f"{high.__str__(level+1)} "
         else:
             ret += "h:[None] "
 
         low = self._context._id_to_node.get(self._low, None)
         if low is not None:
-            ret += "\n" + "\t" * (level + 1) + f" {low.__str__(level + 1)} "
+            ret += "\n" + "\t" * (level + 1) + f"{low.__str__(level + 1)} "
         else:
             ret += "h:[None] "
-        ret += "\n) "
+        ret += "\n" + "\t" * level + ") "
         return ret
 
     def to_graph(self, graph: Graph, node_id: int):
         # Decision node
         this_node = str(node_id)
         graph.add_node(this_node)
         dec_id = self.dec
```

### Comparing `xaddpy-0.1.8/xaddpy/xadd/reduce_lp.py` & `xaddpy-0.1.9/xaddpy/xadd/reduce_lp.py`

 * *Files identical despite different names*

### Comparing `xaddpy-0.1.8/xaddpy/xadd/xadd.py` & `xaddpy-0.1.9/xaddpy/xadd/xadd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,26 @@
+import warnings
 from sympy.logic import boolalg
 import sympy
 import sympy.core.numbers as numbers
 import sympy.core.relational as relational
 from sympy import oo, S
 import numpy as np
 from pathlib import Path
 
 import xaddpy.utils.util
 
 try:
     from xaddpy.utils.graph import Graph
 except ImportError:
-    pass
+    warnings.warn("[Module: xaddpy.xadd.xadd] Import error: pygraphviz not installed")
+    class Graph:
+        def __init__(self, *args, **kwargs):
+            pass
+
 
 from xaddpy.xadd.node import Node, XADDINode, XADDTNode
 from xaddpy.xadd.reduce_lp import ReduceLPContext
 import abc
 from xaddpy.utils.global_vars import (
     REL_TYPE, OP_TYPE, UNARY_OP, RELATIONAL_OPERATOR, ACCEPTED_RV_TYPES
 )
@@ -1683,22 +1688,26 @@
         else:
             xadd_as_list = parse_xadd_grammar(xadd_str, ns=locals if locals is not None else {})[1][0]
         node_id = self.build_initial_xadd(xadd_as_list, to_canonical=to_canonical)
         return node_id
 
     def get_graph(self, node_id: int, name: str = '') -> Graph:
         """Creates a graph view of a given node"""
-        graph = Graph(
-            name=name, 
-            directed=True,
-        )
-        root = self.get_exist_node(node_id)
-        root.to_graph(graph, node_id)
-        return graph
-
+        try:
+            graph = Graph(
+                name=name, 
+                directed=True,
+            )
+            root = self.get_exist_node(node_id)
+            root.to_graph(graph, node_id)
+            return graph
+        except AttributeError:
+            warnings.warn("You need to install 'pygraphviz' to construct graph visualization")
+            raise Exception
+        
     def save_graph(self, node_id: int, file_name: str):
         graph = self.get_graph(node_id)
         graph.configure()
         
         f_dir = Path('./tmp')
         f_dir.mkdir(exist_ok=True, parents=True)
         if file_name.endswith('png'):
```

### Comparing `xaddpy-0.1.8/xaddpy/xadd/xadd_parse_utils.py` & `xaddpy-0.1.9/xaddpy/xadd/xadd_parse_utils.py`

 * *Files identical despite different names*

### Comparing `xaddpy-0.1.8/xaddpy.egg-info/PKG-INFO` & `xaddpy-0.1.9/xaddpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: xaddpy
-Version: 0.1.8
+Version: 0.1.9
 Summary: XADD package in Python
 Home-page: https://github.com/jihwan-jeong/xaddpy
-Download-URL: https://github.com/jihwan-jeong/xaddpy/archive/refs/tags/0.1.8.tar.gz
+Download-URL: https://github.com/jihwan-jeong/xaddpy/archive/refs/tags/0.1.9.tar.gz
 Author: Jihwan Jeong
 Author-email: Jihwan Jeong <jiihwan.jeong@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 jihwan-jeong
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

