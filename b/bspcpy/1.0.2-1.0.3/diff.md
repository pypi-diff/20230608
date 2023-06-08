# Comparing `tmp/bspcpy-1.0.2.tar.gz` & `tmp/bspcpy-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bspcpy-1.0.2.tar", last modified: Sun Mar  5 22:02:11 2023, max compression
+gzip compressed data, was "bspcpy-1.0.3.tar", last modified: Thu Jun  8 01:31:20 2023, max compression
```

## Comparing `bspcpy-1.0.2.tar` & `bspcpy-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 alan      (1000) alan      (1000)        0 2023-03-05 22:02:11.335792 bspcpy-1.0.2/
--rw-r--r--   0 alan      (1000) alan      (1000)     1067 2023-03-04 03:09:52.000000 bspcpy-1.0.2/LICENCE
--rw-r--r--   0 alan      (1000) alan      (1000)     1714 2023-03-05 22:02:11.339125 bspcpy-1.0.2/PKG-INFO
--rw-r--r--   0 alan      (1000) alan      (1000)     1347 2023-03-04 03:19:34.000000 bspcpy-1.0.2/README.md
-drwxr-xr-x   0 alan      (1000) alan      (1000)        0 2023-03-05 22:02:11.335792 bspcpy-1.0.2/bspc/
--rw-r--r--   0 alan      (1000) alan      (1000)       51 2023-03-04 03:09:52.000000 bspcpy-1.0.2/bspc/__init__.py
--rw-r--r--   0 alan      (1000) alan      (1000)    11889 2023-03-05 21:51:42.000000 bspcpy-1.0.2/bspc/classes.py
--rw-r--r--   0 alan      (1000) alan      (1000)      794 2023-03-04 03:09:52.000000 bspcpy-1.0.2/bspc/query.py
-drwxr-xr-x   0 alan      (1000) alan      (1000)        0 2023-03-05 22:02:11.335792 bspcpy-1.0.2/bspcpy.egg-info/
--rw-r--r--   0 alan      (1000) alan      (1000)     1714 2023-03-05 22:02:11.000000 bspcpy-1.0.2/bspcpy.egg-info/PKG-INFO
--rw-r--r--   0 alan      (1000) alan      (1000)      218 2023-03-05 22:02:11.000000 bspcpy-1.0.2/bspcpy.egg-info/SOURCES.txt
--rw-r--r--   0 alan      (1000) alan      (1000)        1 2023-03-05 22:02:11.000000 bspcpy-1.0.2/bspcpy.egg-info/dependency_links.txt
--rw-r--r--   0 alan      (1000) alan      (1000)        5 2023-03-05 22:02:11.000000 bspcpy-1.0.2/bspcpy.egg-info/top_level.txt
--rw-r--r--   0 alan      (1000) alan      (1000)      442 2023-03-05 21:58:21.000000 bspcpy-1.0.2/pyproject.toml
--rw-r--r--   0 alan      (1000) alan      (1000)       79 2023-03-05 22:02:11.339125 bspcpy-1.0.2/setup.cfg
--rw-r--r--   0 alan      (1000) alan      (1000)      342 2023-03-04 03:09:52.000000 bspcpy-1.0.2/setup.py
+drwxr-xr-x   0 alan      (1000) alan      (1000)        0 2023-06-08 01:31:20.125227 bspcpy-1.0.3/
+-rw-r--r--   0 alan      (1000) alan      (1000)     1067 2023-04-03 19:03:41.000000 bspcpy-1.0.3/LICENSE
+-rw-r--r--   0 alan      (1000) alan      (1000)     2959 2023-06-08 01:31:20.125227 bspcpy-1.0.3/PKG-INFO
+-rw-r--r--   0 alan      (1000) alan      (1000)     1347 2023-03-04 03:19:34.000000 bspcpy-1.0.3/README.md
+drwxr-xr-x   0 alan      (1000) alan      (1000)        0 2023-06-08 01:31:20.125227 bspcpy-1.0.3/bspc/
+-rw-r--r--   0 alan      (1000) alan      (1000)       79 2023-06-08 01:21:34.000000 bspcpy-1.0.3/bspc/__init__.py
+-rw-r--r--   0 alan      (1000) alan      (1000)    12757 2023-03-22 01:14:02.000000 bspcpy-1.0.3/bspc/classes.py
+-rw-r--r--   0 alan      (1000) alan      (1000)     2079 2023-03-22 01:08:33.000000 bspcpy-1.0.3/bspc/query.py
+drwxr-xr-x   0 alan      (1000) alan      (1000)        0 2023-06-08 01:31:20.125227 bspcpy-1.0.3/bspcpy.egg-info/
+-rw-r--r--   0 alan      (1000) alan      (1000)     2959 2023-06-08 01:31:20.000000 bspcpy-1.0.3/bspcpy.egg-info/PKG-INFO
+-rw-r--r--   0 alan      (1000) alan      (1000)      218 2023-06-08 01:31:20.000000 bspcpy-1.0.3/bspcpy.egg-info/SOURCES.txt
+-rw-r--r--   0 alan      (1000) alan      (1000)        1 2023-06-08 01:31:20.000000 bspcpy-1.0.3/bspcpy.egg-info/dependency_links.txt
+-rw-r--r--   0 alan      (1000) alan      (1000)        5 2023-06-08 01:31:20.000000 bspcpy-1.0.3/bspcpy.egg-info/top_level.txt
+-rw-r--r--   0 alan      (1000) alan      (1000)      442 2023-06-08 01:31:05.000000 bspcpy-1.0.3/pyproject.toml
+-rw-r--r--   0 alan      (1000) alan      (1000)       79 2023-06-08 01:31:20.125227 bspcpy-1.0.3/setup.cfg
+-rw-r--r--   0 alan      (1000) alan      (1000)      342 2023-03-04 03:09:52.000000 bspcpy-1.0.3/setup.py
```

### Comparing `bspcpy-1.0.2/LICENCE` & `bspcpy-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bspcpy-1.0.2/README.md` & `bspcpy-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `bspcpy-1.0.2/bspc/classes.py` & `bspcpy-1.0.3/bspc/classes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from __future__ import annotations
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Generic, TypeVar
 if TYPE_CHECKING:
     from _typeshed import SupportsRichComparison
 import subprocess
 import json
 from typing import Iterable, Literal, TypedDict, Callable
 from operator import attrgetter
 from copy import copy
@@ -64,69 +64,82 @@
     userLayout:str
     windowGap:int
     borderWidth:int
     focusedNodeId:int
     padding:padding_type
     root:node_type
 
-class Node_set():
-    def __init__(self, iterator:Iterable['Node'], ordered=False):
-        self._set:set[Node] = set(iterator)
+T = TypeVar('T', bound='Node|Desktop|Monitor')
+
+class Element_set(Generic[T]):
+    def __init__(self, iterator:Iterable['T'], ordered=False):
+        self._set:set[T] = set(iterator)
         self.ordered = ordered
 
-    def pop(self) -> 'Node|None':
+    def pop(self) -> 'T|None':
         if not len(self._set):
             return None
         return max(self._set, key=attrgetter('index'))
-    def first(self) -> 'Node|None':
+    def first(self) -> 'T|None':
         if not len(self._set):
             return None
         return min(self._set, key=attrgetter('index'))
 
-    def next(self, node:'Node|None') -> 'Node|None':
+    def next(self, node:'T|None') -> 'T|None':
         if not node:
             return None
 
         next_node = next((item for item in sorted(self._set, key=lambda x:x.index) if item.index > node.index and item != node),None) 
 
         return next_node or self.first()
 
-    def filter(self, callback:Callable[['Node'], bool]):
+    def filter(self, callback:Callable[['T'], bool]):
         new_set = copy(self._set)
         for item in self._set:
             if not callback(item):
                 new_set.remove(item)
-        return Node_set(new_set, ordered=self.ordered)
+        return Element_set(new_set, ordered=self.ordered)
     
-    def sort(self, key:Callable[['Node'], SupportsRichComparison], reverse=False):
+    def sort(self, key:Callable[['T'], SupportsRichComparison], reverse=False):
         self.ordered = True
         for i,node in enumerate(sorted(self._set, key=key, reverse=reverse)):
             node.__dict__['index'] = i
         return self
 
-    def intersection(self, other:'Node_set'):
-        return Node_set(self._set.intersection(other), ordered=self.ordered)
-    def difference(self, other:'Node_set'):
-        return Node_set(self._set.difference(other), ordered=self.ordered)
-    def __and__(self, other:'Node_set'):
-        return Node_set(self._set.intersection(other), ordered=self.ordered)
-    def __sub__(self, other:'Node_set'):
-        return Node_set(self._set.difference(other), ordered=self.ordered)
+    def intersection(self, other:'Element_set'):
+        return Element_set(self._set.intersection(other), ordered=self.ordered)
+    def difference(self, other:'Element_set'):
+        return Element_set(self._set.difference(other), ordered=self.ordered)
+    def __and__(self, other:'Element_set'):
+        return Element_set(self._set.intersection(other), ordered=self.ordered)
+    def __sub__(self, other:'Element_set'):
+        return Element_set(self._set.difference(other), ordered=self.ordered)
     def __iter__(self):
         return iter(self._set)
     def __repr__(self):
         return repr(self._set)
     def __bool__(self):
         return bool(self._set)
 
+class Node_set(Element_set['Node']):
+    def __init__(self, iterator:Iterable['Node'], ordered=False):
+        super().__init__(iterator, ordered)
+class Desktop_set(Element_set['Desktop']):
+    def __init__(self, iterator:Iterable['Desktop'], ordered=False):
+        super().__init__(iterator, ordered)
+class Monitor_set(Element_set['Monitor']):
+    def __init__(self, iterator:Iterable['Monitor'], ordered=False):
+        super().__init__(iterator, ordered)
+
 class Node:
     def __init__(self, id:int, index=-1):
+        self.id:int
         self.index:int
+        self.__dict__['id'] = id
         self.__dict__['index'] = index
-        self.id:int
         self.className:str
         self.layout:str
 
         self.splitType: str
         self.splitRatio: float
         self.vacant: bool
         self.hidden: bool
@@ -137,15 +150,18 @@
         self.presel: str
         self.rectangle: rectangle_type
         self.constraints: constraints_type
         self.firstChild: node_type|None
         self.secondChild: node_type|None
         self.client: client_type|None
 
-        result = subprocess.run(['bspc', 'query','-T', '-n', hex(id)], capture_output=True, text=True)
+        self.refresh()
+
+    def refresh(self):
+        result = subprocess.run(['bspc', 'query','-T', '-n', hex(self.id)], capture_output=True, text=True)
 
         data = json.loads(result.stdout)
         for item in data:
             self.__dict__[item] = data[item]
 
         if self.client:
             self.__dict__['className'] = self.client['className']
@@ -175,17 +191,17 @@
         elif name == 'layout' and value in WINDOW_STATES:
             self.state(value)
         else:
             raise Exception('invalid property')
 
     @property
     def name(self):
-        result = subprocess.run(['xwininfo', '-id', hex(self.id)], check=True, capture_output=True)
-        result = subprocess.run(['head', '-n2'], input=result.stdout, check=True, capture_output=True)
-        result = subprocess.run(['grep', r'\"(.+)\"', '-E', '-o'], input=result.stdout, check=True, capture_output=True)
+        result = subprocess.run(['xwininfo', '-id', hex(self.id)], check=False, capture_output=True)
+        result = subprocess.run(['head', '-n2'], input=result.stdout, check=False, capture_output=True)
+        result = subprocess.run(['grep', r'\"(.+)\"', '-E', '-o'], input=result.stdout, check=False, capture_output=True)
 
         win_name = result.stdout.decode().strip()
         if win_name:
             win_name = win_name[1:-1]
 
         return win_name
 
@@ -264,25 +280,29 @@
         else:
             self.command(f'--to-desktop {selector} {"--follow" if follow else ""}')
 
 
 class Desktop:
     def __init__(self, id:int):
         self.id:int
+        self.index:int
+        self.__dict__['id'] = id
+        self.__dict__['index'] = 0
 
         self.name:str
         self.layout:str
         self.userLayout:str
         self.windowGap:int
         self.borderWidth:int
         self.focusedNodeId:int
         self.padding:padding_type
         self.root:node_type
 
-        result = subprocess.run(['bspc', 'query','-T', '-d', hex(id)], capture_output=True, text=True)
+    def refresh(self):
+        result = subprocess.run(['bspc', 'query','-T', '-d', hex(self.id)], capture_output=True, text=True)
 
         data = json.loads(result.stdout)
         for item in data:
             self.__dict__[item] = data[item]
 
     def __setattr__(self):
         raise Exception('invalid property')
@@ -328,27 +348,31 @@
     def set_layout(self, name:Literal['forward', 'backward', 'monocle', 'tiled']):
         self.command(f'--layout {name}')
 
 
 class Monitor:
     def __init__(self, id:int):
         self.id:int
+        self.index:int
+        self.__dict__['id'] = id
+        self.__dict__['index'] = 0
 
         self.name:str
         self.randrId:int
         self.wired:bool
         self.stickyCount:int
         self.windowGap:int
         self.borderWidth:int
         self.focusedDesktopId:int
         self.padding:padding_type
         self.rectangle:rectangle_type
         self.desktops:list[desktop_type]
 
-        result = subprocess.run(['bspc', 'query','-T', '-m', hex(id)], capture_output=True, text=True)
+    def refresh(self):
+        result = subprocess.run(['bspc', 'query','-T', '-m', hex(self.id)], capture_output=True, text=True)
 
         data = json.loads(result.stdout)
         for item in data:
             self.__dict__[item] = data[item]
 
     def __setattr__(self):
         raise Exception('invalid property')
```

