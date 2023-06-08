# Comparing `tmp/pyrena-1.1.8.tar.gz` & `tmp/pyrena-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrena-1.1.8.tar", last modified: Tue Sep  6 18:51:49 2022, max compression
+gzip compressed data, was "pyrena-1.1.9.tar", last modified: Tue Sep  6 20:01:48 2022, max compression
```

## Comparing `pyrena-1.1.8.tar` & `pyrena-1.1.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2022-09-06 18:51:49.255419 pyrena-1.1.8/
--rw-rw-rw-   0        0        0     1077 2022-08-03 18:04:59.000000 pyrena-1.1.8/LICENSE.txt
--rw-rw-rw-   0        0        0     1365 2022-09-06 18:51:49.254419 pyrena-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1145 2022-08-04 15:50:28.000000 pyrena-1.1.8/README.md
-drwxrwxrwx   0        0        0        0 2022-09-06 18:51:49.238419 pyrena-1.1.8/pyrena/
--rw-rw-rw-   0        0        0    17920 2022-09-06 18:48:26.000000 pyrena-1.1.8/pyrena/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-06 18:51:49.254419 pyrena-1.1.8/pyrena/classes/
--rw-rw-rw-   0        0        0      374 2022-08-09 14:25:32.000000 pyrena-1.1.8/pyrena/classes/__init__.py
--rw-rw-rw-   0        0        0     9272 2022-09-06 18:41:33.000000 pyrena-1.1.8/pyrena/classes/base.py
--rw-rw-rw-   0        0        0      637 2022-08-03 20:21:48.000000 pyrena-1.1.8/pyrena/classes/bom.py
--rw-rw-rw-   0        0        0     3909 2022-08-09 13:17:11.000000 pyrena-1.1.8/pyrena/classes/change.py
--rw-rw-rw-   0        0        0     2844 2022-08-03 20:21:36.000000 pyrena-1.1.8/pyrena/classes/eventqueue.py
--rw-rw-rw-   0        0        0      112 2022-07-29 17:42:48.000000 pyrena-1.1.8/pyrena/classes/extract.py
--rw-rw-rw-   0        0        0     3292 2022-09-06 18:27:13.000000 pyrena-1.1.8/pyrena/classes/file.py
--rw-rw-rw-   0        0        0     2555 2022-08-08 18:19:07.000000 pyrena-1.1.8/pyrena/classes/item.py
--rw-rw-rw-   0        0        0     7449 2022-09-06 18:51:17.000000 pyrena-1.1.8/pyrena/classes/quality.py
--rw-rw-rw-   0        0        0     1943 2022-08-08 18:21:30.000000 pyrena-1.1.8/pyrena/classes/supplier.py
--rw-rw-rw-   0        0        0     3407 2022-08-09 14:36:00.000000 pyrena-1.1.8/pyrena/classes/tickets.py
--rw-rw-rw-   0        0        0     3475 2022-08-19 14:57:46.000000 pyrena-1.1.8/pyrena/classes/training.py
--rw-rw-rw-   0        0        0      473 2022-08-03 20:22:24.000000 pyrena-1.1.8/pyrena/classes/user.py
-drwxrwxrwx   0        0        0        0 2022-09-06 18:51:49.244454 pyrena-1.1.8/pyrena.egg-info/
--rw-rw-rw-   0        0        0     1365 2022-09-06 18:51:49.000000 pyrena-1.1.8/pyrena.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      525 2022-09-06 18:51:49.000000 pyrena-1.1.8/pyrena.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-06 18:51:49.000000 pyrena-1.1.8/pyrena.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2022-09-06 18:51:49.000000 pyrena-1.1.8/pyrena.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-09-06 18:51:49.000000 pyrena-1.1.8/pyrena.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-09-06 18:51:49.255419 pyrena-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0      480 2022-09-06 18:51:40.000000 pyrena-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-09-06 20:01:48.072085 pyrena-1.1.9/
+-rw-rw-rw-   0        0        0     1077 2022-08-03 18:04:59.000000 pyrena-1.1.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     1365 2022-09-06 20:01:48.071085 pyrena-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1145 2022-08-04 15:50:28.000000 pyrena-1.1.9/README.md
+drwxrwxrwx   0        0        0        0 2022-09-06 20:01:48.050462 pyrena-1.1.9/pyrena/
+-rw-rw-rw-   0        0        0    17943 2022-09-06 20:01:21.000000 pyrena-1.1.9/pyrena/__init__.py
+drwxrwxrwx   0        0        0        0 2022-09-06 20:01:48.070084 pyrena-1.1.9/pyrena/classes/
+-rw-rw-rw-   0        0        0      374 2022-08-09 14:25:32.000000 pyrena-1.1.9/pyrena/classes/__init__.py
+-rw-rw-rw-   0        0        0     9272 2022-09-06 18:41:33.000000 pyrena-1.1.9/pyrena/classes/base.py
+-rw-rw-rw-   0        0        0      637 2022-08-03 20:21:48.000000 pyrena-1.1.9/pyrena/classes/bom.py
+-rw-rw-rw-   0        0        0     3909 2022-08-09 13:17:11.000000 pyrena-1.1.9/pyrena/classes/change.py
+-rw-rw-rw-   0        0        0     2844 2022-08-03 20:21:36.000000 pyrena-1.1.9/pyrena/classes/eventqueue.py
+-rw-rw-rw-   0        0        0      112 2022-07-29 17:42:48.000000 pyrena-1.1.9/pyrena/classes/extract.py
+-rw-rw-rw-   0        0        0     3292 2022-09-06 18:27:13.000000 pyrena-1.1.9/pyrena/classes/file.py
+-rw-rw-rw-   0        0        0     2555 2022-08-08 18:19:07.000000 pyrena-1.1.9/pyrena/classes/item.py
+-rw-rw-rw-   0        0        0     7449 2022-09-06 18:51:17.000000 pyrena-1.1.9/pyrena/classes/quality.py
+-rw-rw-rw-   0        0        0     1943 2022-08-08 18:21:30.000000 pyrena-1.1.9/pyrena/classes/supplier.py
+-rw-rw-rw-   0        0        0     3407 2022-08-09 14:36:00.000000 pyrena-1.1.9/pyrena/classes/tickets.py
+-rw-rw-rw-   0        0        0     3475 2022-08-19 14:57:46.000000 pyrena-1.1.9/pyrena/classes/training.py
+-rw-rw-rw-   0        0        0      473 2022-08-03 20:22:24.000000 pyrena-1.1.9/pyrena/classes/user.py
+drwxrwxrwx   0        0        0        0 2022-09-06 20:01:48.054462 pyrena-1.1.9/pyrena.egg-info/
+-rw-rw-rw-   0        0        0     1365 2022-09-06 20:01:48.000000 pyrena-1.1.9/pyrena.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      525 2022-09-06 20:01:48.000000 pyrena-1.1.9/pyrena.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-09-06 20:01:48.000000 pyrena-1.1.9/pyrena.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2022-09-06 20:01:48.000000 pyrena-1.1.9/pyrena.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2022-09-06 20:01:48.000000 pyrena-1.1.9/pyrena.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-09-06 20:01:48.072085 pyrena-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      480 2022-09-06 20:01:34.000000 pyrena-1.1.9/setup.py
```

### Comparing `pyrena-1.1.8/LICENSE.txt` & `pyrena-1.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyrena-1.1.8/PKG-INFO` & `pyrena-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrena
-Version: 1.1.8
+Version: 1.1.9
 Summary: Python wrapper for Arena QMS API.
 Home-page: https://github.com/thecodeforge/pyrena
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # pyrena
```

### Comparing `pyrena-1.1.8/README.md` & `pyrena-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pyrena-1.1.8/pyrena/__init__.py` & `pyrena-1.1.9/pyrena/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -376,15 +376,15 @@
 
         - folder    - Path to existing archive folder, if one already exists
         - exclude   - list of Arena classes to exclude from the backup.
         """
 
         d= time.strftime("%d_%B_%Y")
 
-        folder_name = folder_name or f"Arena_archive_{d}"
+        folder_name = folder_name or f"Arena_archive_{self._workspace_name}_{d}"
 
         if not os.path.exists(folder_name):
             os.mkdir(folder_name)
 
         #Files
         if self.File not in exclude:
```

### Comparing `pyrena-1.1.8/pyrena/classes/base.py` & `pyrena-1.1.9/pyrena/classes/base.py`

 * *Files identical despite different names*

### Comparing `pyrena-1.1.8/pyrena/classes/bom.py` & `pyrena-1.1.9/pyrena/classes/bom.py`

 * *Files identical despite different names*

### Comparing `pyrena-1.1.8/pyrena/classes/change.py` & `pyrena-1.1.9/pyrena/classes/change.py`

 * *Files identical despite different names*

### Comparing `pyrena-1.1.8/pyrena/classes/eventqueue.py` & `pyrena-1.1.9/pyrena/classes/eventqueue.py`

 * *Files identical despite different names*

### Comparing `pyrena-1.1.8/pyrena/classes/file.py` & `pyrena-1.1.9/pyrena/classes/file.py`

 * *Files identical despite different names*

### Comparing `pyrena-1.1.8/pyrena/classes/item.py` & `pyrena-1.1.9/pyrena/classes/item.py`

 * *Files identical despite different names*

### Comparing `pyrena-1.1.8/pyrena/classes/quality.py` & `pyrena-1.1.9/pyrena/classes/quality.py`

 * *Files identical despite different names*

### Comparing `pyrena-1.1.8/pyrena/classes/supplier.py` & `pyrena-1.1.9/pyrena/classes/supplier.py`

 * *Files identical despite different names*

### Comparing `pyrena-1.1.8/pyrena/classes/tickets.py` & `pyrena-1.1.9/pyrena/classes/tickets.py`

 * *Files identical despite different names*

### Comparing `pyrena-1.1.8/pyrena/classes/training.py` & `pyrena-1.1.9/pyrena/classes/training.py`

 * *Files identical despite different names*

### Comparing `pyrena-1.1.8/pyrena.egg-info/PKG-INFO` & `pyrena-1.1.9/pyrena.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrena
-Version: 1.1.8
+Version: 1.1.9
 Summary: Python wrapper for Arena QMS API.
 Home-page: https://github.com/thecodeforge/pyrena
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # pyrena
```

### Comparing `pyrena-1.1.8/pyrena.egg-info/SOURCES.txt` & `pyrena-1.1.9/pyrena.egg-info/SOURCES.txt`

 * *Files identical despite different names*

