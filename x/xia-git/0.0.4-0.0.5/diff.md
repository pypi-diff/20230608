# Comparing `tmp/xia_git-0.0.4-cp39-none-win_amd64.whl.zip` & `tmp/xia_git-0.0.5-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 111832 bytes, number of entries: 7
--rw-r--r--  2.0 unx       76 b- defN 23-Jun-08 11:18 xia_git/__init__.py
--rw-r--r--  2.0 unx   269312 b- defN 23-Jun-08 11:21 xia_git/git.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-08 11:21 xia_git-0.0.4.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      625 b- defN 23-Jun-08 11:21 xia_git-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-08 11:21 xia_git-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jun-08 11:21 xia_git-0.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      550 b- defN 23-Jun-08 11:21 xia_git-0.0.4.dist-info/RECORD
-7 files, 270821 bytes uncompressed, 110854 bytes compressed:  59.1%
+Zip file size: 112074 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-08 14:21 xia_git/__init__.py
+-rw-r--r--  2.0 unx   269312 b- defN 23-Jun-08 14:24 xia_git/git.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-08 14:24 xia_git-0.0.5.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      625 b- defN 23-Jun-08 14:24 xia_git-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-08 14:24 xia_git-0.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-08 14:24 xia_git-0.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      550 b- defN 23-Jun-08 14:24 xia_git-0.0.5.dist-info/RECORD
+7 files, 270821 bytes uncompressed, 111096 bytes compressed:  59.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_git/__init__.py
 Comment: 
 
 Filename: xia_git/git.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_git-0.0.4.dist-info/LICENSE.txt
+Filename: xia_git-0.0.5.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_git-0.0.4.dist-info/METADATA
+Filename: xia_git-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: xia_git-0.0.4.dist-info/WHEEL
+Filename: xia_git-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: xia_git-0.0.4.dist-info/top_level.txt
+Filename: xia_git-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_git-0.0.4.dist-info/RECORD
+Filename: xia_git-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_git/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_git.git import Git
 
 __all__ = [
     "Git"
 ]
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
```

## Comparing `xia_git-0.0.4.dist-info/METADATA` & `xia_git-0.0.5.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-git
-Version: 0.0.4
+Version: 0.0.5
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-git/0.0.4/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-git/0.0.5/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

