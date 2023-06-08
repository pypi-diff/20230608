# Comparing `tmp/lbuild-1.9.1.tar.gz` & `tmp/lbuild-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lbuild-1.9.1.tar", last modified: Fri Mar  1 20:55:13 2019, max compression
+gzip compressed data, was "dist/lbuild-1.9.2.tar", last modified: Tue Mar 12 22:31:36 2019, max compression
```

## Comparing `lbuild-1.9.1.tar` & `lbuild-1.9.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-01 20:55:13.000000 lbuild-1.9.1/
--rw-rw-r--   0 travis    (2000) travis    (2000)    41172 2019-03-01 20:54:52.000000 lbuild-1.9.1/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     1296 2019-03-01 20:54:52.000000 lbuild-1.9.1/LICENSE.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     2076 2019-03-01 20:54:52.000000 lbuild-1.9.1/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-01 20:55:13.000000 lbuild-1.9.1/lbuild/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1915 2019-03-01 20:54:52.000000 lbuild-1.9.1/lbuild/query.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11930 2019-03-01 20:54:52.000000 lbuild-1.9.1/lbuild/option.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17197 2019-03-01 20:54:52.000000 lbuild-1.9.1/lbuild/main.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14180 2019-03-01 20:54:52.000000 lbuild-1.9.1/lbuild/facade.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3958 2019-03-01 20:54:52.000000 lbuild-1.9.1/lbuild/collector.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3843 2019-03-01 20:54:52.000000 lbuild-1.9.1/lbuild/api.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      815 2019-03-01 20:54:52.000000 lbuild-1.9.1/lbuild/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8657 2019-03-01 20:54:52.000000 lbuild-1.9.1/lbuild/format.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8430 2019-03-01 20:54:52.000000 lbuild-1.9.1/lbuild/config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9938 2019-03-01 20:54:52.000000 lbuild-1.9.1/lbuild/buildlog.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10721 2019-03-01 20:54:52.000000 lbuild-1.9.1/lbuild/parser.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-01 20:55:13.000000 lbuild-1.9.1/lbuild/resources/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3279 2019-03-01 20:54:52.000000 lbuild-1.9.1/lbuild/resources/configuration.xsd
--rw-rw-r--   0 travis    (2000) travis    (2000)     2274 2019-03-01 20:54:52.000000 lbuild-1.9.1/lbuild/exception.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1192 2019-03-01 20:54:52.000000 lbuild-1.9.1/lbuild/logger.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6323 2019-03-01 20:54:52.000000 lbuild-1.9.1/lbuild/repository.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16478 2019-03-01 20:54:52.000000 lbuild-1.9.1/lbuild/environment.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5699 2019-03-01 20:54:52.000000 lbuild-1.9.1/lbuild/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-01 20:55:13.000000 lbuild-1.9.1/lbuild/builder/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3222 2019-03-01 20:54:52.000000 lbuild-1.9.1/lbuild/builder/dependency.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2019-03-01 20:54:52.000000 lbuild-1.9.1/lbuild/builder/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7488 2019-03-01 20:54:52.000000 lbuild-1.9.1/lbuild/module.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1617 2019-03-01 20:54:52.000000 lbuild-1.9.1/lbuild/filter.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-01 20:55:13.000000 lbuild-1.9.1/lbuild/vcs/
--rw-rw-r--   0 travis    (2000) travis    (2000)      315 2019-03-01 20:54:52.000000 lbuild-1.9.1/lbuild/vcs/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1220 2019-03-01 20:54:52.000000 lbuild-1.9.1/lbuild/vcs/common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2482 2019-03-01 20:54:52.000000 lbuild-1.9.1/lbuild/vcs/git.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17614 2019-03-01 20:54:52.000000 lbuild-1.9.1/lbuild/node.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-03-01 20:55:13.000000 lbuild-1.9.1/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      154 2019-03-01 20:54:52.000000 lbuild-1.9.1/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       45 2019-03-01 20:54:52.000000 lbuild-1.9.1/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)    50972 2019-03-01 20:55:13.000000 lbuild-1.9.1/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-01 20:55:13.000000 lbuild-1.9.1/lbuild.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)        7 2019-03-01 20:55:13.000000 lbuild-1.9.1/lbuild.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       91 2019-03-01 20:55:13.000000 lbuild-1.9.1/lbuild.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    50972 2019-03-01 20:55:13.000000 lbuild-1.9.1/lbuild.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-03-01 20:55:13.000000 lbuild-1.9.1/lbuild.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       45 2019-03-01 20:55:13.000000 lbuild-1.9.1/lbuild.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      727 2019-03-01 20:55:13.000000 lbuild-1.9.1/lbuild.egg-info/SOURCES.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-12 22:31:36.000000 lbuild-1.9.2/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41172 2019-03-12 22:31:13.000000 lbuild-1.9.2/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1296 2019-03-12 22:31:13.000000 lbuild-1.9.2/LICENSE.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2076 2019-03-12 22:31:13.000000 lbuild-1.9.2/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-12 22:31:36.000000 lbuild-1.9.2/lbuild/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1915 2019-03-12 22:31:13.000000 lbuild-1.9.2/lbuild/query.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11930 2019-03-12 22:31:13.000000 lbuild-1.9.2/lbuild/option.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17213 2019-03-12 22:31:13.000000 lbuild-1.9.2/lbuild/main.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14180 2019-03-12 22:31:13.000000 lbuild-1.9.2/lbuild/facade.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3958 2019-03-12 22:31:13.000000 lbuild-1.9.2/lbuild/collector.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3843 2019-03-12 22:31:13.000000 lbuild-1.9.2/lbuild/api.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      815 2019-03-12 22:31:13.000000 lbuild-1.9.2/lbuild/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8440 2019-03-12 22:31:13.000000 lbuild-1.9.2/lbuild/format.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8430 2019-03-12 22:31:13.000000 lbuild-1.9.2/lbuild/config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9938 2019-03-12 22:31:13.000000 lbuild-1.9.2/lbuild/buildlog.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10721 2019-03-12 22:31:13.000000 lbuild-1.9.2/lbuild/parser.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-12 22:31:36.000000 lbuild-1.9.2/lbuild/resources/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3279 2019-03-12 22:31:13.000000 lbuild-1.9.2/lbuild/resources/configuration.xsd
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2274 2019-03-12 22:31:13.000000 lbuild-1.9.2/lbuild/exception.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1192 2019-03-12 22:31:13.000000 lbuild-1.9.2/lbuild/logger.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6323 2019-03-12 22:31:13.000000 lbuild-1.9.2/lbuild/repository.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16478 2019-03-12 22:31:13.000000 lbuild-1.9.2/lbuild/environment.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5699 2019-03-12 22:31:13.000000 lbuild-1.9.2/lbuild/utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-12 22:31:36.000000 lbuild-1.9.2/lbuild/builder/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3222 2019-03-12 22:31:13.000000 lbuild-1.9.2/lbuild/builder/dependency.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2019-03-12 22:31:13.000000 lbuild-1.9.2/lbuild/builder/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7488 2019-03-12 22:31:13.000000 lbuild-1.9.2/lbuild/module.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1617 2019-03-12 22:31:13.000000 lbuild-1.9.2/lbuild/filter.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-12 22:31:36.000000 lbuild-1.9.2/lbuild/vcs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      315 2019-03-12 22:31:13.000000 lbuild-1.9.2/lbuild/vcs/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1220 2019-03-12 22:31:13.000000 lbuild-1.9.2/lbuild/vcs/common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2482 2019-03-12 22:31:13.000000 lbuild-1.9.2/lbuild/vcs/git.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17614 2019-03-12 22:31:13.000000 lbuild-1.9.2/lbuild/node.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-03-12 22:31:36.000000 lbuild-1.9.2/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      154 2019-03-12 22:31:13.000000 lbuild-1.9.2/requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       45 2019-03-12 22:31:13.000000 lbuild-1.9.2/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)    50972 2019-03-12 22:31:36.000000 lbuild-1.9.2/PKG-INFO
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-12 22:31:36.000000 lbuild-1.9.2/lbuild.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        7 2019-03-12 22:31:36.000000 lbuild-1.9.2/lbuild.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       91 2019-03-12 22:31:36.000000 lbuild-1.9.2/lbuild.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    50972 2019-03-12 22:31:36.000000 lbuild-1.9.2/lbuild.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-03-12 22:31:36.000000 lbuild-1.9.2/lbuild.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       45 2019-03-12 22:31:36.000000 lbuild-1.9.2/lbuild.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      727 2019-03-12 22:31:36.000000 lbuild-1.9.2/lbuild.egg-info/SOURCES.txt
```

### Comparing `lbuild-1.9.1/README.md` & `lbuild-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `lbuild-1.9.1/LICENSE.txt` & `lbuild-1.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lbuild-1.9.1/setup.py` & `lbuild-1.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `lbuild-1.9.1/lbuild/query.py` & `lbuild-1.9.2/lbuild/query.py`

 * *Files identical despite different names*

### Comparing `lbuild-1.9.1/lbuild/option.py` & `lbuild-1.9.2/lbuild/option.py`

 * *Files identical despite different names*

### Comparing `lbuild-1.9.1/lbuild/main.py` & `lbuild-1.9.2/lbuild/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,22 +10,23 @@
 # governing this code.
 
 import os
 import re
 import sys
 import argparse
 import traceback
+import textwrap
 
 import lbuild.logger
 import lbuild.vcs.common
 from lbuild.format import format_option_short_description
 
 from lbuild.api import Builder
 
-__version__ = '1.9.1'
+__version__ = '1.9.2'
 
 
 class InitAction:
 
     def register(self, argument_parser):
         parser = argument_parser.add_parser(
             "init",
```

### Comparing `lbuild-1.9.1/lbuild/facade.py` & `lbuild-1.9.2/lbuild/facade.py`

 * *Files identical despite different names*

### Comparing `lbuild-1.9.1/lbuild/collector.py` & `lbuild-1.9.2/lbuild/collector.py`

 * *Files identical despite different names*

### Comparing `lbuild-1.9.1/lbuild/api.py` & `lbuild-1.9.2/lbuild/api.py`

 * *Files identical despite different names*

### Comparing `lbuild-1.9.1/lbuild/__init__.py` & `lbuild-1.9.2/lbuild/__init__.py`

 * *Files identical despite different names*

### Comparing `lbuild-1.9.1/lbuild/format.py` & `lbuild-1.9.2/lbuild/format.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,30 +220,30 @@
 
 
 def format_short_description(_, description):
     lines = description.strip().splitlines() + [""]
     return lines[0].strip().rstrip(".,:;!?")
 
 
-def format_node(node, _):
+def format_node(node, _, depth):
     name = _cw(node.name)
     class_name = _cw(node.class_name)
     if node._type == node.Type.REPOSITORY:
         name = _cw(node.name + " @ " + os.path.relpath(node._filepath, os.getcwd()))
     elif node._type == node.Type.OPTION:
         name = format_option_name(node, fullname=False)
     elif node._type in [node.Type.MODULE, node.Type.CONFIG]:
         name = _cw(node.fullname).wrap(node)
     elif node._type in [node.Type.QUERY, node.Type.COLLECTOR]:
         class_name = class_name.wrap("underlined")
         name = name.wrap("bold")
 
     descr = (class_name + _cw("(") + name + _cw(")")).wrap(node)
 
-    offset = node.depth * 4
+    offset = (node.depth - depth) * 4
     if node._type == node.Type.OPTION:
         descr += _cw(" = ")
         descr += format_option_value_description(node, offset=offset + len(descr), single_line=True)
     elif node._type == node.Type.COLLECTOR:
         descr += _cw(" in [")
         descr += format_option_values(node, offset=offset + len(descr), single_line=True)
         descr += _cw("]")
@@ -253,25 +253,18 @@
     return descr.limit(offset)
 
 
 def format_node_tree(node, filterfunc=None):
     if filterfunc is None:
         filterfunc = lambda n: n.type in SHOW_NODES
 
-    class Renderer(anytree.RenderTree):
-        def __init__(self, node):
-            anytree.RenderTree.__init__(self, node,
-                                        style=anytree.ContRoundStyle(),
-                                        childiter=self.childiter)
-
-        @staticmethod
-        def childiter(nodes):
-            nodes = [n for n in nodes if filterfunc(n)]
-            return sorted(nodes, key=lambda node: (node._type, node.name))
-
-        def __str__(self):
-            lines = []
-            for pre, _, node in self:
-                lines.append(pre + format_node(node, pre))
-            return "\n".join(lines)
-
-    return str(Renderer(node))
+    def childiter(nodes):
+        nodes = [n for n in nodes if filterfunc(n)]
+        return sorted(nodes, key=lambda node: (node._type, node.name))
+
+    depth = node.depth
+    render = anytree.RenderTree(node, childiter=childiter,
+                                style=anytree.ContRoundStyle())
+    lines = []
+    for pre, _, node in render:
+        lines.append(pre + format_node(node, pre, depth))
+    return "\n".join(lines)
```

### Comparing `lbuild-1.9.1/lbuild/config.py` & `lbuild-1.9.2/lbuild/config.py`

 * *Files identical despite different names*

### Comparing `lbuild-1.9.1/lbuild/buildlog.py` & `lbuild-1.9.2/lbuild/buildlog.py`

 * *Files identical despite different names*

### Comparing `lbuild-1.9.1/lbuild/parser.py` & `lbuild-1.9.2/lbuild/parser.py`

 * *Files identical despite different names*

### Comparing `lbuild-1.9.1/lbuild/resources/configuration.xsd` & `lbuild-1.9.2/lbuild/resources/configuration.xsd`

 * *Files identical despite different names*

### Comparing `lbuild-1.9.1/lbuild/exception.py` & `lbuild-1.9.2/lbuild/exception.py`

 * *Files identical despite different names*

### Comparing `lbuild-1.9.1/lbuild/logger.py` & `lbuild-1.9.2/lbuild/logger.py`

 * *Files identical despite different names*

### Comparing `lbuild-1.9.1/lbuild/repository.py` & `lbuild-1.9.2/lbuild/repository.py`

 * *Files identical despite different names*

### Comparing `lbuild-1.9.1/lbuild/environment.py` & `lbuild-1.9.2/lbuild/environment.py`

 * *Files identical despite different names*

### Comparing `lbuild-1.9.1/lbuild/utils.py` & `lbuild-1.9.2/lbuild/utils.py`

 * *Files identical despite different names*

### Comparing `lbuild-1.9.1/lbuild/builder/dependency.py` & `lbuild-1.9.2/lbuild/builder/dependency.py`

 * *Files identical despite different names*

### Comparing `lbuild-1.9.1/lbuild/module.py` & `lbuild-1.9.2/lbuild/module.py`

 * *Files identical despite different names*

### Comparing `lbuild-1.9.1/lbuild/filter.py` & `lbuild-1.9.2/lbuild/filter.py`

 * *Files identical despite different names*

### Comparing `lbuild-1.9.1/lbuild/vcs/common.py` & `lbuild-1.9.2/lbuild/vcs/common.py`

 * *Files identical despite different names*

### Comparing `lbuild-1.9.1/lbuild/vcs/git.py` & `lbuild-1.9.2/lbuild/vcs/git.py`

 * *Files identical despite different names*

### Comparing `lbuild-1.9.1/lbuild/node.py` & `lbuild-1.9.2/lbuild/node.py`

 * *Files identical despite different names*

### Comparing `lbuild-1.9.1/PKG-INFO` & `lbuild-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbuild
-Version: 1.9.1
+Version: 1.9.2
 Summary: Generic, modular code generator using the Jinja2 template engine.
 Home-page: https://github.com/modm-io/lbuild
 Author: Fabian Greif, Niklas Hauser
 Author-email: fabian.greif@rwth-aachen.de, niklas@salkinium.com
 License: BSD
 Description: # lbuild: generic, modular code generation in Python 3 [![][travis-svg]][travis]
```

### Comparing `lbuild-1.9.1/lbuild.egg-info/PKG-INFO` & `lbuild-1.9.2/lbuild.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbuild
-Version: 1.9.1
+Version: 1.9.2
 Summary: Generic, modular code generator using the Jinja2 template engine.
 Home-page: https://github.com/modm-io/lbuild
 Author: Fabian Greif, Niklas Hauser
 Author-email: fabian.greif@rwth-aachen.de, niklas@salkinium.com
 License: BSD
 Description: # lbuild: generic, modular code generation in Python 3 [![][travis-svg]][travis]
```

### Comparing `lbuild-1.9.1/lbuild.egg-info/SOURCES.txt` & `lbuild-1.9.2/lbuild.egg-info/SOURCES.txt`

 * *Files identical despite different names*

