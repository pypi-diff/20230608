# Comparing `tmp/JestingLang-0.0.0a4.tar.gz` & `tmp/JestingLang-0.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JestingLang-0.0.0a4.tar", last modified: Sat May 27 13:59:02 2023, max compression
+gzip compressed data, was "JestingLang-0.0.0a5.tar", last modified: Thu Jun  8 13:53:00 2023, max compression
```

## Comparing `JestingLang-0.0.0a4.tar` & `JestingLang-0.0.0a5.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-27 13:59:02.618116 JestingLang-0.0.0a4/
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1085 2023-05-09 15:44:29.000000 JestingLang-0.0.0a4/LICENSE
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)      937 2023-05-27 13:59:02.618116 JestingLang-0.0.0a4/PKG-INFO
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1467 2023-05-22 15:41:51.000000 JestingLang-0.0.0a4/README.md
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)      103 2023-05-27 13:59:02.635496 JestingLang-0.0.0a4/setup.cfg
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1274 2023-05-27 13:58:43.000000 JestingLang-0.0.0a4/setup.py
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-27 13:59:01.345734 JestingLang-0.0.0a4/src/
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-27 13:59:01.550307 JestingLang-0.0.0a4/src/JestingLang/
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-27 13:59:01.942697 JestingLang-0.0.0a4/src/JestingLang/JParsing/
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     4255 2023-05-22 15:24:28.000000 JestingLang-0.0.0a4/src/JestingLang/JParsing/JestingAST.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     5221 2023-05-27 13:58:43.000000 JestingLang-0.0.0a4/src/JestingLang/JParsing/LexerParser.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     9898 2023-05-15 07:17:19.000000 JestingLang-0.0.0a4/src/JestingLang/JParsing/LexerParser_cachedParseTable.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-25 16:59:49.000000 JestingLang-0.0.0a4/src/JestingLang/JParsing/__init__.py
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-27 13:59:02.162385 JestingLang-0.0.0a4/src/JestingLang/JVisitors/
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)      760 2023-05-15 07:35:03.000000 JestingLang-0.0.0a4/src/JestingLang/JVisitors/AbstractJestingVisitor.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1083 2023-05-27 13:58:43.000000 JestingLang-0.0.0a4/src/JestingLang/JVisitors/ContextBoundInterpreterVisitor.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     2649 2023-05-27 13:58:43.000000 JestingLang-0.0.0a4/src/JestingLang/JVisitors/ContextfreeInterpreterVisitor.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     2588 2023-05-27 13:58:43.000000 JestingLang-0.0.0a4/src/JestingLang/JVisitors/PrettyPrintingVisitors.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-15 07:17:36.000000 JestingLang-0.0.0a4/src/JestingLang/JVisitors/__init__.py
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-27 13:59:02.224885 JestingLang-0.0.0a4/src/JestingLang/Misc/
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-27 13:59:02.367167 JestingLang-0.0.0a4/src/JestingLang/Misc/JContext/
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)      243 2023-05-22 14:21:19.000000 JestingLang-0.0.0a4/src/JestingLang/Misc/JContext/AbstractContext.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)      859 2023-05-27 13:58:43.000000 JestingLang-0.0.0a4/src/JestingLang/Misc/JContext/MapContext.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-15 07:20:09.000000 JestingLang-0.0.0a4/src/JestingLang/Misc/JContext/__init__.py
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-27 13:59:02.429667 JestingLang-0.0.0a4/src/JestingLang/Misc/JExample/
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-22 14:14:47.000000 JestingLang-0.0.0a4/src/JestingLang/Misc/JExample/__init__.py
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-27 13:59:02.586866 JestingLang-0.0.0a4/src/JestingLang/Misc/JLogic/
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1404 2023-05-22 14:56:31.000000 JestingLang-0.0.0a4/src/JestingLang/Misc/JLogic/LogicFunctions.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     2527 2023-05-27 13:58:43.000000 JestingLang-0.0.0a4/src/JestingLang/Misc/JLogic/OperationMapping.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-15 06:01:19.000000 JestingLang-0.0.0a4/src/JestingLang/Misc/JLogic/__init__.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-22 12:31:24.000000 JestingLang-0.0.0a4/src/JestingLang/Misc/__init__.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-15 06:05:46.000000 JestingLang-0.0.0a4/src/JestingLang/__init__.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     2702 2023-05-27 13:58:43.000000 JestingLang-0.0.0a4/src/JestingLang/main.py
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-27 13:59:01.769980 JestingLang-0.0.0a4/src/JestingLang.egg-info/
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)      937 2023-05-27 13:59:00.000000 JestingLang-0.0.0a4/src/JestingLang.egg-info/PKG-INFO
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1060 2023-05-27 13:59:01.000000 JestingLang-0.0.0a4/src/JestingLang.egg-info/SOURCES.txt
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)        1 2023-05-27 13:59:00.000000 JestingLang-0.0.0a4/src/JestingLang.egg-info/dependency_links.txt
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)        4 2023-05-27 13:59:00.000000 JestingLang-0.0.0a4/src/JestingLang.egg-info/requires.txt
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)       12 2023-05-27 13:59:00.000000 JestingLang-0.0.0a4/src/JestingLang.egg-info/top_level.txt
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-08 13:53:00.159461 JestingLang-0.0.0a5/
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1085 2023-05-09 15:44:29.000000 JestingLang-0.0.0a5/LICENSE
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)      937 2023-06-08 13:53:00.166579 JestingLang-0.0.0a5/PKG-INFO
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     2096 2023-06-08 13:25:42.000000 JestingLang-0.0.0a5/README.md
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)      103 2023-06-08 13:53:00.176799 JestingLang-0.0.0a5/setup.cfg
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1274 2023-06-08 13:26:44.000000 JestingLang-0.0.0a5/setup.py
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-08 13:52:58.136732 JestingLang-0.0.0a5/src/
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-08 13:52:58.440333 JestingLang-0.0.0a5/src/JestingLang/
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-08 13:52:59.000300 JestingLang-0.0.0a5/src/JestingLang/JParsing/
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     4326 2023-06-08 13:15:01.000000 JestingLang-0.0.0a5/src/JestingLang/JParsing/JestingAST.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     5221 2023-05-27 13:58:43.000000 JestingLang-0.0.0a5/src/JestingLang/JParsing/LexerParser.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     9898 2023-05-15 07:17:19.000000 JestingLang-0.0.0a5/src/JestingLang/JParsing/LexerParser_cachedParseTable.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-25 16:59:49.000000 JestingLang-0.0.0a5/src/JestingLang/JParsing/__init__.py
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-08 13:52:59.356833 JestingLang-0.0.0a5/src/JestingLang/JVisitors/
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)      816 2023-05-28 16:16:17.000000 JestingLang-0.0.0a5/src/JestingLang/JVisitors/AbstractJestingVisitor.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1371 2023-06-08 12:33:56.000000 JestingLang-0.0.0a5/src/JestingLang/JVisitors/ContextBoundInterpreterVisitor.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     2998 2023-06-08 13:07:54.000000 JestingLang-0.0.0a5/src/JestingLang/JVisitors/ContextfreeInterpreterVisitor.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     2588 2023-05-27 13:58:43.000000 JestingLang-0.0.0a5/src/JestingLang/JVisitors/PrettyPrintingVisitors.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-15 07:17:36.000000 JestingLang-0.0.0a5/src/JestingLang/JVisitors/__init__.py
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-08 13:52:59.426563 JestingLang-0.0.0a5/src/JestingLang/Misc/
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-08 13:52:59.759865 JestingLang-0.0.0a5/src/JestingLang/Misc/JContext/
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)      243 2023-06-08 08:56:27.000000 JestingLang-0.0.0a5/src/JestingLang/Misc/JContext/AbstractContext.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1291 2023-05-28 16:06:05.000000 JestingLang-0.0.0a5/src/JestingLang/Misc/JContext/MapContext.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1403 2023-06-08 12:42:00.000000 JestingLang-0.0.0a5/src/JestingLang/Misc/JContext/MemoryContext.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-15 07:20:09.000000 JestingLang-0.0.0a5/src/JestingLang/Misc/JContext/__init__.py
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-08 13:52:59.836713 JestingLang-0.0.0a5/src/JestingLang/Misc/JExample/
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-22 14:14:47.000000 JestingLang-0.0.0a5/src/JestingLang/Misc/JExample/__init__.py
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-08 13:53:00.086793 JestingLang-0.0.0a5/src/JestingLang/Misc/JLogic/
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1430 2023-06-08 11:18:42.000000 JestingLang-0.0.0a5/src/JestingLang/Misc/JLogic/LogicFunctions.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     2629 2023-06-08 13:12:55.000000 JestingLang-0.0.0a5/src/JestingLang/Misc/JLogic/OperationMapping.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-15 06:01:19.000000 JestingLang-0.0.0a5/src/JestingLang/Misc/JLogic/__init__.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-22 12:31:24.000000 JestingLang-0.0.0a5/src/JestingLang/Misc/__init__.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-15 06:05:46.000000 JestingLang-0.0.0a5/src/JestingLang/__init__.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     2702 2023-05-27 13:58:43.000000 JestingLang-0.0.0a5/src/JestingLang/main.py
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-08 13:52:58.716675 JestingLang-0.0.0a5/src/JestingLang.egg-info/
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)      937 2023-06-08 13:52:57.000000 JestingLang-0.0.0a5/src/JestingLang.egg-info/PKG-INFO
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1107 2023-06-08 13:52:58.000000 JestingLang-0.0.0a5/src/JestingLang.egg-info/SOURCES.txt
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        1 2023-06-08 13:52:57.000000 JestingLang-0.0.0a5/src/JestingLang.egg-info/dependency_links.txt
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        4 2023-06-08 13:52:57.000000 JestingLang-0.0.0a5/src/JestingLang.egg-info/requires.txt
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)       12 2023-06-08 13:52:57.000000 JestingLang-0.0.0a5/src/JestingLang.egg-info/top_level.txt
```

### Comparing `JestingLang-0.0.0a4/LICENSE` & `JestingLang-0.0.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `JestingLang-0.0.0a4/PKG-INFO` & `JestingLang-0.0.0a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JestingLang
-Version: 0.0.0a4
+Version: 0.0.0a5
 Summary: A compiler for the minimalist spreadsheet language Jesting
 Home-page: https://github.com/itruffat/JestingLang
 Author: itrufat
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `JestingLang-0.0.0a4/README.md` & `JestingLang-0.0.0a5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -33,10 +33,24 @@
     = INDIRECT("A" & 2) -> becomes an indirection to cell A2
     = IF(0 = 0 , 2 , 3) -> becomes 3
 
 The AST can become more complex, with nodes such as 
 *EmptyValue* or *DateValue*. However, they can be easily
 solved by using the Visitors provided in this library.
 
+# Fixed vs Volatile Visitors
+
+Some APPS using JestingLang may need to precompile a tree 
+without actually resolving values and references, as the 
+value of a cell may get updated data every once in a while 
+without updating the formula behind it. With that in mind,
+the concept of **volatile** was included in this lib. 
+
+A volatile Node is one such that it has (or includes or some 
+sub-branch that has) a value that is not fixed. In turn, a 
+volatile visitor is one that resolves all volatile nodes 
+when visiting a tree. A fixed tree does the opposite, and 
+returns a Tree without exploring any volatile Node. 
+
 # TODO
 
 * Finish dates
```

### Comparing `JestingLang-0.0.0a4/setup.py` & `JestingLang-0.0.0a5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='JestingLang',
-    version='0.0.0a4',
+    version='0.0.0a5',
     author='itrufat',
     description='A compiler for the minimalist spreadsheet language Jesting',
     long_description='A compiler + a few node navigators (including an interpreter) for a minimalist language intended to copy the most basic functionalities found in spreadsheet-applications called JestingLang. It was created to be used with Jesting, a spreadsheet terminal tool.',
     long_description_content_type='text/markdown',
     url='https://github.com/itruffat/JestingLang',
     packages=['JestingLang', 'JestingLang.JParsing', 'JestingLang.JVisitors', 'JestingLang.Misc',
               'JestingLang.Misc.JLogic', 'JestingLang.Misc.JContext', 'JestingLang.Misc.JExample'],
```

### Comparing `JestingLang-0.0.0a4/src/JestingLang/JParsing/JestingAST.py` & `JestingLang-0.0.0a5/src/JestingLang/JParsing/JestingAST.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,18 +22,19 @@
 
     def accept(self, visitor):
         return visitor.visitSimple(self)
 
 
 class EmptyValueNode(SimpleValueNode):
     def __init__(self):
-        super().__init__("")
+        super().__init__(None)
 
     def accept(self, visitor):
-        return visitor.visitEmpty(self)
+        child = visitor.visitEmpty(self)
+        return super().accept(visitor) if child is None else child
 
     def volatile(self):
         return False
 
 
 class InnerError():
```

### Comparing `JestingLang-0.0.0a4/src/JestingLang/JParsing/LexerParser.py` & `JestingLang-0.0.0a5/src/JestingLang/JParsing/LexerParser.py`

 * *Files identical despite different names*

### Comparing `JestingLang-0.0.0a4/src/JestingLang/JParsing/LexerParser_cachedParseTable.py` & `JestingLang-0.0.0a5/src/JestingLang/JParsing/LexerParser_cachedParseTable.py`

 * *Files identical despite different names*

### Comparing `JestingLang-0.0.0a4/src/JestingLang/JVisitors/AbstractJestingVisitor.py` & `JestingLang-0.0.0a5/src/JestingLang/JVisitors/AbstractJestingVisitor.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,17 @@
     def visit(self, node):
         return node.accept(self)
 
     @abstractmethod
     def visitSimple(self, node):
         return None
 
+    def visitEmpty(self, node):
+        return None
+
     def visitInvalid(self, node):
         return None
 
     def visitStr(self, node):
         return None
 
     def visitInt(self, node):
```

### Comparing `JestingLang-0.0.0a4/src/JestingLang/JVisitors/ContextBoundInterpreterVisitor.py` & `JestingLang-0.0.0a5/src/JestingLang/JVisitors/ContextBoundInterpreterVisitor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,29 @@
-from JestingLang.JParsing.JestingAST import InvalidValueNode, ReferenceValueNode
+from JestingLang.JParsing.JestingAST import InvalidValueNode, ReferenceValueNode, IndirectNode
 from JestingLang.Misc.JLogic.LogicFunctions import ref
 from JestingLang.JVisitors.ContextfreeInterpreterVisitor import ContextfreeInterpreterVisitor
 
 
 class ContextBoundInterpreterVisitor(ContextfreeInterpreterVisitor):
 
     """The complete syntax resolver, it requires a reference resolver to get the references when visiting stuff"""
-    def __init__(self, context):
-        super().__init__()
+    def __init__(self, context, resolveVolatile):
+        super().__init__(resolveVolatile)
         self.contextResolver = context
 
     def visitRef(self, node):
-        referenced = self.contextResolver.resolve(node.value)
-        return InvalidValueNode("Broken reference") if referenced is None else referenced
+        if node.volatile and (not self.resolveVolatile):
+            return node
+        referencedNode = self.contextResolver.resolve(node.value)
+        return InvalidValueNode("Broken reference") if referencedNode is None else referencedNode.accept(self)
 
     def visitIndirect(self, node):
         children_visited = node.children[0].accept(self)
-        if children_visited.volatile():
-            return children_visited
+        if (not self.resolveVolatile) and children_visited.volatile():
+            return IndirectNode(children_visited)
         reference = ref(children_visited.value)
         if reference is None:
             return InvalidValueNode("Bad reference")
+        if not self.resolveVolatile:
+            return IndirectNode(children_visited)
         return ReferenceValueNode(reference).accept(self)
```

### Comparing `JestingLang-0.0.0a4/src/JestingLang/JVisitors/ContextfreeInterpreterVisitor.py` & `JestingLang-0.0.0a5/src/JestingLang/JVisitors/ContextfreeInterpreterVisitor.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,48 +16,54 @@
         return BoolValueNode(bool(value))
 
 
 class ContextfreeInterpreterVisitor(AbstractJestingVisitor):
 
     """The basic resolver for the syntax, does not depend on anything besides itself but can't resolve references"""
 
+    def __init__(self, resolveVolatile):
+        super().__init__()
+        self.resolveVolatile = resolveVolatile
+
     def visit(self, node):
         return node.accept(self)
 
     def visitSimple(self, node):
         return node
 
     def visitOperation(self, node):
         visitedChildren = {k: v.accept(self) for k, v in node.children.items()}
-        if any(map(lambda c:c.volatile(), visitedChildren.values())):
+        if not self.resolveVolatile and any(map(lambda c:c.volatile(), visitedChildren.values())):
             answer = OperationNode(node.operation, visitedChildren)
         else:
             variables = {k : v.value for k,v in visitedChildren.items()}
             errors, value, label = operations[node.operation](variables = variables)
             if len(errors) == 0:
                 answer = renodify(value, label)
             else:
                 answer = InvalidValueNode(",".join(errors))
         return answer
 
     def visitIf(self, node):
         _if = node.children[0].accept(self)
-        _then = node.children[1].accept(self)
-        _else = node.children[2].accept(self)
 
-        if _if.volatile():
-            answer = IfNode(_if,_then,_else)
+        if not self.resolveVolatile and _if.volatile():
+            _then = node.children[1].accept(self)
+            _else = node.children[2].accept(self)
+            answer = IfNode(_if, _then, _else)
         else:
             # This behaviour is not real since spreedsheets don't use short-circuit (for whatever reason)
-            if boolean(_if.value) and not _then.volatile():
-               answer = _then
-            elif not boolean(_if.value) and not _else.volatile():
-                answer = _else
+            if boolean(_if.value):
+                # if boolean(_if.value) and (self.resolveVolatile or not _then.volatile()):
+                _then = node.children[1].accept(self)
+                answer = _then
             else:
-                answer = IfNode(_if,_then,_else)
+                # elif not boolean(_if.value) and (self.resolveVolatile or not _else.volatile()):
+                _else = node.children[2].accept(self)
+                answer = _else
 
         return answer
 
     def visitRef(self, node):
         return ToleratedErrorNode(node.value, "CONTEXT FREE, NOT IMPLEMENTED")
 
     def visitIndirect(self, node):
```

### Comparing `JestingLang-0.0.0a4/src/JestingLang/JVisitors/PrettyPrintingVisitors.py` & `JestingLang-0.0.0a5/src/JestingLang/JVisitors/PrettyPrintingVisitors.py`

 * *Files identical despite different names*

### Comparing `JestingLang-0.0.0a4/src/JestingLang/Misc/JContext/MapContext.py` & `JestingLang-0.0.0a5/src/JestingLang/Misc/JContext/MapContext.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-from Misc.JContext.AbstractContext import AbstractContext
-from JestingLang.JParsing.JestingAST import SimpleValueNode
+from JestingLang.Misc.JContext.AbstractContext import AbstractContext
+from JestingLang.JParsing.JestingAST import SimpleValueNode, Node, StrValueNode, IntValueNode
 
 
 class MapContext(AbstractContext):
-    """Example of a context, in this case by using a map for formulas respectively"""
+    """Example of a context, in this case by using a map for formulas respectively.
+    This context does not support circular recursion and will freeze when trying to solve it.
+    It also returns an error value if an unknown name is given."""
 
     def __init__(self):
         super().__init__()
         self.formulas = {}
 
     def resolve(self, name):
         if name not in self.formulas.keys():
@@ -17,13 +19,20 @@
     def valueOf(self, node):
         if issubclass(type(node), SimpleValueNode):
             value = node.value
         else:
             value = node
         return value
 
-    def write(self, key, value):
-        self.formulas[key] = value
+    def write(self, key, formula):
+        assert(issubclass(type(formula), Node))
+        self.formulas[key] =formula
+
+    def writeNumber(self, key, value):
+        self.write(key, IntValueNode(value))
+
+    def writeStr(self, key, value):
+        self.write(key, StrValueNode(value))
 
     def show(self):
         _keys = set(self.formulas.keys())
         return {key: self.valueOf(self.resolve(key)) for key in _keys}
```

### Comparing `JestingLang-0.0.0a4/src/JestingLang/Misc/JLogic/LogicFunctions.py` & `JestingLang-0.0.0a5/src/JestingLang/Misc/JLogic/LogicFunctions.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     #   return True
     if digit.match(str(pseudo_boolean)):
         return int(pseudo_boolean) < 0
     return None
 
 
 def integer(pseudo_integer):
-    if pseudo_integer == "":
+    if pseudo_integer == "" or pseudo_integer is None:
         return 0
     else:
         if digit.match(str(pseudo_integer)):
             return int(pseudo_integer)
     return None
 
 def ref(pseudo_ref):
```

### Comparing `JestingLang-0.0.0a4/src/JestingLang/Misc/JLogic/OperationMapping.py` & `JestingLang-0.0.0a5/src/JestingLang/Misc/JLogic/OperationMapping.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from Misc.JLogic.LogicFunctions import variablesIntoIntegers
+from JestingLang.Misc.JLogic.LogicFunctions import variablesIntoIntegers
 from JestingLang.JParsing.JestingAST import operations as astOperations
 
 def operationPlus(variables):
     variables_int, errors = variablesIntoIntegers(variables, "Plus(+)")
     answer = 0
     if len(errors) == 0:
         answer = variables_int[0] + variables_int[1]
@@ -34,15 +34,16 @@
     if str(variables[1]) == "0":
         errors.append("Divided by zero")
     if len(errors) == 0:
         answer = variables_int[0] / variables_int[1]
     return errors, answer, "INT"
 
 def operationConcat(variables):
-    return [], str(variables[0]) + str(variables[1]), "STR"
+    return [], str(variables[0] if variables[0] is not None else '') + \
+               str(variables[1] if variables[1] is not None else ''), "STR"
 
 
 def operationEquals(variables):
     print(variables)
     return [], variables[0] == variables[1], "BOOL" # Needs further improving
 
 def operationAnd(variables):
```

### Comparing `JestingLang-0.0.0a4/src/JestingLang/main.py` & `JestingLang-0.0.0a5/src/JestingLang/main.py`

 * *Files identical despite different names*

### Comparing `JestingLang-0.0.0a4/src/JestingLang.egg-info/PKG-INFO` & `JestingLang-0.0.0a5/src/JestingLang.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JestingLang
-Version: 0.0.0a4
+Version: 0.0.0a5
 Summary: A compiler for the minimalist spreadsheet language Jesting
 Home-page: https://github.com/itruffat/JestingLang
 Author: itrufat
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `JestingLang-0.0.0a4/src/JestingLang.egg-info/SOURCES.txt` & `JestingLang-0.0.0a5/src/JestingLang.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -17,12 +17,13 @@
 src/JestingLang/JVisitors/ContextBoundInterpreterVisitor.py
 src/JestingLang/JVisitors/ContextfreeInterpreterVisitor.py
 src/JestingLang/JVisitors/PrettyPrintingVisitors.py
 src/JestingLang/JVisitors/__init__.py
 src/JestingLang/Misc/__init__.py
 src/JestingLang/Misc/JContext/AbstractContext.py
 src/JestingLang/Misc/JContext/MapContext.py
+src/JestingLang/Misc/JContext/MemoryContext.py
 src/JestingLang/Misc/JContext/__init__.py
 src/JestingLang/Misc/JExample/__init__.py
 src/JestingLang/Misc/JLogic/LogicFunctions.py
 src/JestingLang/Misc/JLogic/OperationMapping.py
 src/JestingLang/Misc/JLogic/__init__.py
```

