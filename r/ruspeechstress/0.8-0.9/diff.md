# Comparing `tmp/ruspeechstress-0.8.tar.gz` & `tmp/ruspeechstress-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ruspeechstress-0.8.tar", last modified: Wed Jun  7 16:34:16 2023, max compression
+gzip compressed data, was "ruspeechstress-0.9.tar", last modified: Wed Jun  7 16:38:08 2023, max compression
```

## Comparing `ruspeechstress-0.8.tar` & `ruspeechstress-0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 sivh      (1000) sivh      (1000)        0 2023-06-07 16:34:16.047209 ruspeechstress-0.8/
--rw-rw-r--   0 sivh      (1000) sivh      (1000)      303 2023-06-07 16:34:16.047209 ruspeechstress-0.8/PKG-INFO
-drwxrwxr-x   0 sivh      (1000) sivh      (1000)        0 2023-06-07 16:34:16.047209 ruspeechstress-0.8/ruspeechstress/
--rw-rw-r--   0 sivh      (1000) sivh      (1000)      747 2023-06-07 16:33:38.000000 ruspeechstress-0.8/ruspeechstress/__init__.py
--rw-rw-r--   0 sivh      (1000) sivh      (1000)    13536 2023-06-07 16:33:38.000000 ruspeechstress-0.8/ruspeechstress/dataset.py
--rw-rw-r--   0 sivh      (1000) sivh      (1000)    31206 2023-06-07 09:32:56.000000 ruspeechstress-0.8/ruspeechstress/sound.py
--rw-rw-r--   0 sivh      (1000) sivh      (1000)    18830 2023-06-07 16:12:22.000000 ruspeechstress-0.8/ruspeechstress/stress_detector.py
--rw-rw-r--   0 sivh      (1000) sivh      (1000)     1806 2021-06-01 18:24:40.000000 ruspeechstress-0.8/ruspeechstress/utils.py
-drwxrwxr-x   0 sivh      (1000) sivh      (1000)        0 2023-06-07 16:34:16.047209 ruspeechstress-0.8/ruspeechstress.egg-info/
--rw-rw-r--   0 sivh      (1000) sivh      (1000)      303 2023-06-07 16:34:16.000000 ruspeechstress-0.8/ruspeechstress.egg-info/PKG-INFO
--rw-rw-r--   0 sivh      (1000) sivh      (1000)      295 2023-06-07 16:34:16.000000 ruspeechstress-0.8/ruspeechstress.egg-info/SOURCES.txt
--rw-rw-r--   0 sivh      (1000) sivh      (1000)        1 2023-06-07 16:34:16.000000 ruspeechstress-0.8/ruspeechstress.egg-info/dependency_links.txt
--rw-rw-r--   0 sivh      (1000) sivh      (1000)       15 2023-06-07 16:34:16.000000 ruspeechstress-0.8/ruspeechstress.egg-info/top_level.txt
--rw-rw-r--   0 sivh      (1000) sivh      (1000)       38 2023-06-07 16:34:16.047209 ruspeechstress-0.8/setup.cfg
--rw-rw-r--   0 sivh      (1000) sivh      (1000)      377 2023-06-07 16:33:48.000000 ruspeechstress-0.8/setup.py
+drwxrwxr-x   0 sivh      (1000) sivh      (1000)        0 2023-06-07 16:38:08.915605 ruspeechstress-0.9/
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)      303 2023-06-07 16:38:08.915605 ruspeechstress-0.9/PKG-INFO
+drwxrwxr-x   0 sivh      (1000) sivh      (1000)        0 2023-06-07 16:38:08.911605 ruspeechstress-0.9/ruspeechstress/
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)      747 2023-06-07 16:33:38.000000 ruspeechstress-0.9/ruspeechstress/__init__.py
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)    13454 2023-06-07 16:37:14.000000 ruspeechstress-0.9/ruspeechstress/dataset.py
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)    31206 2023-06-07 09:32:56.000000 ruspeechstress-0.9/ruspeechstress/sound.py
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)    18830 2023-06-07 16:12:22.000000 ruspeechstress-0.9/ruspeechstress/stress_detector.py
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)     1806 2021-06-01 18:24:40.000000 ruspeechstress-0.9/ruspeechstress/utils.py
+drwxrwxr-x   0 sivh      (1000) sivh      (1000)        0 2023-06-07 16:38:08.915605 ruspeechstress-0.9/ruspeechstress.egg-info/
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)      303 2023-06-07 16:38:08.000000 ruspeechstress-0.9/ruspeechstress.egg-info/PKG-INFO
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)      295 2023-06-07 16:38:08.000000 ruspeechstress-0.9/ruspeechstress.egg-info/SOURCES.txt
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)        1 2023-06-07 16:38:08.000000 ruspeechstress-0.9/ruspeechstress.egg-info/dependency_links.txt
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)       15 2023-06-07 16:38:08.000000 ruspeechstress-0.9/ruspeechstress.egg-info/top_level.txt
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)       38 2023-06-07 16:38:08.915605 ruspeechstress-0.9/setup.cfg
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)      377 2023-06-07 16:37:36.000000 ruspeechstress-0.9/setup.py
```

### Comparing `ruspeechstress-0.8/ruspeechstress/__init__.py` & `ruspeechstress-0.9/ruspeechstress/__init__.py`

 * *Files identical despite different names*

### Comparing `ruspeechstress-0.8/ruspeechstress/dataset.py` & `ruspeechstress-0.9/ruspeechstress/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,20 +28,19 @@
         pass
     else:
         files = os.listdir(os.path.join(working_dir, directory))
         for file in files:
             os.remove(os.path.join(os.path.join(working_dir, directory), file))
 
 
-def get_files(working_dir, input_directory='./dataset'):
+def get_files(working_dir):
     file_pairs = {}
-    full_path = os.path.join(working_dir, input_directory)
-    for file in listdir(full_path):
-        text = os.path.join(full_path, file[:-4] + '.txt')
-        wav = os.path.join(full_path, file)
+    for file in listdir(working_dir):
+        text = os.path.join(working_dir, file[:-4] + '.txt')
+        wav = os.path.join(working_dir, file)
         if file.endswith('.wav') and os.path.exists(text):
             file_pairs.update({wav: text})
         elif file.endswith('.wav') and not os.path.exists(text):
             file_pairs.update({wav: None})
     return file_pairs
```

### Comparing `ruspeechstress-0.8/ruspeechstress/sound.py` & `ruspeechstress-0.9/ruspeechstress/sound.py`

 * *Files identical despite different names*

### Comparing `ruspeechstress-0.8/ruspeechstress/stress_detector.py` & `ruspeechstress-0.9/ruspeechstress/stress_detector.py`

 * *Files identical despite different names*

### Comparing `ruspeechstress-0.8/ruspeechstress/utils.py` & `ruspeechstress-0.9/ruspeechstress/utils.py`

 * *Files identical despite different names*

