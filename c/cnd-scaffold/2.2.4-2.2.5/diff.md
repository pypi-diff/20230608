# Comparing `tmp/cnd_scaffold-2.2.4-py3-none-any.whl.zip` & `tmp/cnd_scaffold-2.2.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4562 bytes, number of entries: 8
--rw-rw-rw-  2.0 unx        5 b- defN 23-Apr-19 23:20 cnd_scaffold/VERSION
--rw-r--r--  2.0 unx      129 b- defN 23-Apr-19 23:20 cnd_scaffold/__init__.py
--rw-r--r--  2.0 unx      121 b- defN 23-Apr-19 23:20 cnd_scaffold/__version__.py
--rw-r--r--  2.0 unx     6764 b- defN 23-Apr-19 23:20 cnd_scaffold/cnd_scaffold.py
--rw-r--r--  2.0 unx     2517 b- defN 23-Apr-19 23:20 cnd_scaffold-2.2.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-19 23:20 cnd_scaffold-2.2.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 23-Apr-19 23:20 cnd_scaffold-2.2.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      640 b- defN 23-Apr-19 23:20 cnd_scaffold-2.2.4.dist-info/RECORD
-8 files, 10281 bytes uncompressed, 3438 bytes compressed:  66.6%
+Zip file size: 4567 bytes, number of entries: 8
+-rw-rw-rw-  2.0 unx        5 b- defN 23-Jun-08 15:34 cnd_scaffold/VERSION
+-rw-r--r--  2.0 unx      129 b- defN 23-Jun-08 15:34 cnd_scaffold/__init__.py
+-rw-r--r--  2.0 unx      121 b- defN 23-Jun-08 15:34 cnd_scaffold/__version__.py
+-rw-r--r--  2.0 unx     6767 b- defN 23-Jun-08 15:34 cnd_scaffold/cnd_scaffold.py
+-rw-r--r--  2.0 unx     2517 b- defN 23-Jun-08 15:34 cnd_scaffold-2.2.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-08 15:34 cnd_scaffold-2.2.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 23-Jun-08 15:34 cnd_scaffold-2.2.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      640 b- defN 23-Jun-08 15:34 cnd_scaffold-2.2.5.dist-info/RECORD
+8 files, 10284 bytes uncompressed, 3443 bytes compressed:  66.5%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: cnd_scaffold/__version__.py
 Comment: 
 
 Filename: cnd_scaffold/cnd_scaffold.py
 Comment: 
 
-Filename: cnd_scaffold-2.2.4.dist-info/METADATA
+Filename: cnd_scaffold-2.2.5.dist-info/METADATA
 Comment: 
 
-Filename: cnd_scaffold-2.2.4.dist-info/WHEEL
+Filename: cnd_scaffold-2.2.5.dist-info/WHEEL
 Comment: 
 
-Filename: cnd_scaffold-2.2.4.dist-info/top_level.txt
+Filename: cnd_scaffold-2.2.5.dist-info/top_level.txt
 Comment: 
 
-Filename: cnd_scaffold-2.2.4.dist-info/RECORD
+Filename: cnd_scaffold-2.2.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cnd_scaffold/VERSION

```diff
@@ -1 +1 @@
-2.2.4
+2.2.5
```

## cnd_scaffold/cnd_scaffold.py

```diff
@@ -149,8 +149,8 @@
     def init(self):
         return self._apply_step('init')
 
     def build(self):
         return self._apply_step('build')
 
     def runtime(self):
-        return self._apply_step('init')
+        return self._apply_step('runtime')
```

## Comparing `cnd_scaffold-2.2.4.dist-info/METADATA` & `cnd_scaffold-2.2.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnd-scaffold
-Version: 2.2.4
+Version: 2.2.5
 Summary: Tools initiate a new project in git lab, based on a existing definition
 Home-page: https://gitlab.com/changendevops/gitopstoolkit/cnd-scaffold.git
 Author: Denis FABIEN
 Author-email: denis.fabien@changendevops.com
 License: MIT/X11
 Project-URL: Documentation, https://changendevops.com
 Project-URL: Source, https://gitlab.com/changendevops/gitopstoolkit/cnd-scaffold.git
```

