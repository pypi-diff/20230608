# Comparing `tmp/Lurlene-8.tar.gz` & `tmp/Lurlene-9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Lurlene-8.tar", last modified: Sat Oct 10 13:31:33 2020, max compression
+gzip compressed data, was "dist/Lurlene-9.tar", last modified: Sun Oct 25 20:53:16 2020, max compression
```

## Comparing `Lurlene-8.tar` & `Lurlene-9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2020-10-10 13:31:33.000000 Lurlene-8/
-drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2020-10-10 13:31:33.000000 Lurlene-8/lurlene/
--rw-rw-r--   0 arc       (1000) arc       (1000)     2187 2020-03-26 18:56:42.000000 Lurlene-8/lurlene/transform.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     2509 2020-08-15 16:21:06.000000 Lurlene-8/lurlene/util.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     5201 2020-08-02 12:33:46.000000 Lurlene-8/lurlene/context.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      708 2019-11-17 19:08:10.000000 Lurlene-8/lurlene/iface.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1427 2019-11-19 20:56:48.000000 Lurlene-8/lurlene/xtra.py
--rw-rw-r--   0 arc       (1000) arc       (1000)    11090 2020-08-10 20:57:22.000000 Lurlene-8/lurlene/lc.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      996 2020-03-11 20:13:29.000000 Lurlene-8/lurlene/pitches.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     6429 2020-08-25 21:01:37.000000 Lurlene-8/lurlene/parse.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     5494 2020-08-15 16:40:30.000000 Lurlene-8/lurlene/bridge.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     3488 2020-08-02 12:33:46.000000 Lurlene-8/lurlene/osc.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1990 2020-08-10 12:27:48.000000 Lurlene-8/lurlene/__init__.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     5298 2020-10-10 13:31:31.000000 Lurlene-8/setup.py
--rw-rw-r--   0 arc       (1000) arc       (1000)       67 2020-10-10 13:31:33.000000 Lurlene-8/setup.cfg
-drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2020-10-10 13:31:33.000000 Lurlene-8/Lurlene.egg-info/
--rw-rw-r--   0 arc       (1000) arc       (1000)        1 2020-10-10 13:31:32.000000 Lurlene-8/Lurlene.egg-info/dependency_links.txt
--rw-rw-r--   0 arc       (1000) arc       (1000)       47 2020-10-10 13:31:32.000000 Lurlene-8/Lurlene.egg-info/requires.txt
--rw-rw-r--   0 arc       (1000) arc       (1000)       20 2020-10-10 13:31:32.000000 Lurlene-8/Lurlene.egg-info/entry_points.txt
--rw-rw-r--   0 arc       (1000) arc       (1000)      408 2020-10-10 13:31:32.000000 Lurlene-8/Lurlene.egg-info/SOURCES.txt
--rw-rw-r--   0 arc       (1000) arc       (1000)        8 2020-10-10 13:31:32.000000 Lurlene-8/Lurlene.egg-info/top_level.txt
--rw-rw-r--   0 arc       (1000) arc       (1000)      536 2020-10-10 13:31:32.000000 Lurlene-8/Lurlene.egg-info/PKG-INFO
--rw-rw-r--   0 arc       (1000) arc       (1000)      209 2020-01-16 20:38:53.000000 Lurlene-8/README.md
--rw-rw-r--   0 arc       (1000) arc       (1000)      536 2020-10-10 13:31:33.000000 Lurlene-8/PKG-INFO
+drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2020-10-25 20:53:16.000000 Lurlene-9/
+drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2020-10-25 20:53:16.000000 Lurlene-9/lurlene/
+-rw-rw-r--   0 arc       (1000) arc       (1000)     2187 2020-03-26 18:56:42.000000 Lurlene-9/lurlene/transform.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     2509 2020-08-15 16:21:06.000000 Lurlene-9/lurlene/util.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     5201 2020-08-02 12:33:46.000000 Lurlene-9/lurlene/context.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      708 2019-11-17 19:08:10.000000 Lurlene-9/lurlene/iface.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1427 2019-11-19 20:56:48.000000 Lurlene-9/lurlene/xtra.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)    11090 2020-08-10 20:57:22.000000 Lurlene-9/lurlene/lc.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      996 2020-03-11 20:13:29.000000 Lurlene-9/lurlene/pitches.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     6429 2020-08-25 21:01:37.000000 Lurlene-9/lurlene/parse.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     5494 2020-08-15 16:40:30.000000 Lurlene-9/lurlene/bridge.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     3488 2020-08-02 12:33:46.000000 Lurlene-9/lurlene/osc.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1990 2020-08-10 12:27:48.000000 Lurlene-9/lurlene/__init__.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     5298 2020-10-25 20:53:15.000000 Lurlene-9/setup.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)       67 2020-10-25 20:53:16.000000 Lurlene-9/setup.cfg
+drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2020-10-25 20:53:16.000000 Lurlene-9/Lurlene.egg-info/
+-rw-rw-r--   0 arc       (1000) arc       (1000)        1 2020-10-25 20:53:16.000000 Lurlene-9/Lurlene.egg-info/dependency_links.txt
+-rw-rw-r--   0 arc       (1000) arc       (1000)       47 2020-10-25 20:53:16.000000 Lurlene-9/Lurlene.egg-info/requires.txt
+-rw-rw-r--   0 arc       (1000) arc       (1000)       20 2020-10-25 20:53:16.000000 Lurlene-9/Lurlene.egg-info/entry_points.txt
+-rw-rw-r--   0 arc       (1000) arc       (1000)      408 2020-10-25 20:53:16.000000 Lurlene-9/Lurlene.egg-info/SOURCES.txt
+-rw-rw-r--   0 arc       (1000) arc       (1000)        8 2020-10-25 20:53:16.000000 Lurlene-9/Lurlene.egg-info/top_level.txt
+-rw-rw-r--   0 arc       (1000) arc       (1000)      536 2020-10-25 20:53:16.000000 Lurlene-9/Lurlene.egg-info/PKG-INFO
+-rw-rw-r--   0 arc       (1000) arc       (1000)      209 2020-01-16 20:38:53.000000 Lurlene-9/README.md
+-rw-rw-r--   0 arc       (1000) arc       (1000)      536 2020-10-25 20:53:16.000000 Lurlene-9/PKG-INFO
```

### Comparing `Lurlene-8/lurlene/transform.py` & `Lurlene-9/lurlene/transform.py`

 * *Files identical despite different names*

### Comparing `Lurlene-8/lurlene/util.py` & `Lurlene-9/lurlene/util.py`

 * *Files identical despite different names*

### Comparing `Lurlene-8/lurlene/context.py` & `Lurlene-9/lurlene/context.py`

 * *Files identical despite different names*

### Comparing `Lurlene-8/lurlene/iface.py` & `Lurlene-9/lurlene/iface.py`

 * *Files identical despite different names*

### Comparing `Lurlene-8/lurlene/xtra.py` & `Lurlene-9/lurlene/xtra.py`

 * *Files identical despite different names*

### Comparing `Lurlene-8/lurlene/lc.py` & `Lurlene-9/lurlene/lc.py`

 * *Files identical despite different names*

### Comparing `Lurlene-8/lurlene/pitches.py` & `Lurlene-9/lurlene/pitches.py`

 * *Files identical despite different names*

### Comparing `Lurlene-8/lurlene/parse.py` & `Lurlene-9/lurlene/parse.py`

 * *Files identical despite different names*

### Comparing `Lurlene-8/lurlene/bridge.py` & `Lurlene-9/lurlene/bridge.py`

 * *Files identical despite different names*

### Comparing `Lurlene-8/lurlene/osc.py` & `Lurlene-9/lurlene/osc.py`

 * *Files identical despite different names*

### Comparing `Lurlene-8/lurlene/__init__.py` & `Lurlene-9/lurlene/__init__.py`

 * *Files identical despite different names*

### Comparing `Lurlene-8/setup.py` & `Lurlene-9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
 def ext_modules():
     extensions = [path.make_ext() for path in sourceinfo.extpaths]
     return dict(ext_modules = cythonize(extensions)) if extensions else {}
 
 sourceinfo = SourceInfo('.')
 setuptools.setup(
         name = 'Lurlene',
-        version = '8',
+        version = '9',
         description = 'Python-based live-coding language optimised for a small number of channels',
         long_description = long_description(),
         long_description_content_type = 'text/markdown',
         url = 'https://github.com/combatopera/Lurlene',
         author = 'Andrzej Cichocki',
         packages = sourceinfo.packages,
         py_modules = [],
```

### Comparing `Lurlene-8/Lurlene.egg-info/PKG-INFO` & `Lurlene-9/Lurlene.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Lurlene
-Version: 8
+Version: 9
 Summary: Python-based live-coding language optimised for a small number of channels
 Home-page: https://github.com/combatopera/Lurlene
 Author: Andrzej Cichocki
 License: UNKNOWN
 Description: # Lurlene
         Python-based live-coding language optimised for a small number of channels.
```

### Comparing `Lurlene-8/PKG-INFO` & `Lurlene-9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Lurlene
-Version: 8
+Version: 9
 Summary: Python-based live-coding language optimised for a small number of channels
 Home-page: https://github.com/combatopera/Lurlene
 Author: Andrzej Cichocki
 License: UNKNOWN
 Description: # Lurlene
         Python-based live-coding language optimised for a small number of channels.
```

