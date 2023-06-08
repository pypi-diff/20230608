# Comparing `tmp/tarn-0.5.1.tar.gz` & `tmp/tarn-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarn-0.5.1.tar", last modified: Fri May 26 11:27:46 2023, max compression
+gzip compressed data, was "tarn-0.6.0.tar", last modified: Thu Jun  8 11:40:19 2023, max compression
```

## Comparing `tarn-0.5.1.tar` & `tarn-0.6.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:27:46.196085 tarn-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-05-26 11:27:43.000000 tarn-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-26 11:27:43.000000 tarn-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-26 11:27:46.196085 tarn-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-26 11:27:43.000000 tarn-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-26 11:27:43.000000 tarn-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-26 11:27:43.000000 tarn-0.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 11:27:46.196085 tarn-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-26 11:27:43.000000 tarn-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:27:46.188084 tarn-0.5.1/tarn/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:27:46.188084 tarn-0.5.1/tarn/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/cache/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/cache/index.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/cache/pickler.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/cache/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/cache/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/digest.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:27:46.192085 tarn-0.5.1/tarn/local/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/local/disk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/local/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:27:46.192085 tarn-0.5.1/tarn/location/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/location/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/location/disk_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/location/fanout.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/location/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/location/levels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/location/nginx.py
--rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/location/scp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:27:46.192085 tarn-0.5.1/tarn/pickler/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/pickler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/pickler/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/pickler/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:27:46.192085 tarn-0.5.1/tarn/pool/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/pool/hash_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/pool/pickle_key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:27:46.196085 tarn-0.5.1/tarn/remote/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/remote/http.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/remote/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:27:46.196085 tarn-0.5.1/tarn/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/tools/labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/tools/locker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/tools/size.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/tools/usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:27:46.188084 tarn-0.5.1/tarn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-26 11:27:46.000000 tarn-0.5.1/tarn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-26 11:27:46.000000 tarn-0.5.1/tarn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 11:27:46.000000 tarn-0.5.1/tarn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-26 11:27:46.000000 tarn-0.5.1/tarn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-26 11:27:46.000000 tarn-0.5.1/tarn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:40:19.944898 tarn-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-06-08 11:40:16.000000 tarn-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-08 11:40:16.000000 tarn-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-08 11:40:19.944898 tarn-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-08 11:40:16.000000 tarn-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-08 11:40:16.000000 tarn-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-08 11:40:16.000000 tarn-0.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 11:40:19.944898 tarn-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-08 11:40:16.000000 tarn-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:40:19.936898 tarn-0.6.0/tarn/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:40:19.940898 tarn-0.6.0/tarn/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/cache/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/cache/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/cache/pickler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/cache/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/cache/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/digest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:40:19.940898 tarn-0.6.0/tarn/local/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/local/disk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/local/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:40:19.940898 tarn-0.6.0/tarn/location/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/location/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/location/disk_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/location/fanout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/location/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/location/levels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/location/nginx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/location/scp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:40:19.940898 tarn-0.6.0/tarn/pickler/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/pickler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/pickler/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9950 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/pickler/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:40:19.940898 tarn-0.6.0/tarn/pool/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/pool/hash_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/pool/pickle_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:40:19.940898 tarn-0.6.0/tarn/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/remote/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/remote/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:40:19.944898 tarn-0.6.0/tarn/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/tools/labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/tools/locker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/tools/size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/tools/usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:40:19.940898 tarn-0.6.0/tarn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-08 11:40:19.000000 tarn-0.6.0/tarn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-08 11:40:19.000000 tarn-0.6.0/tarn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 11:40:19.000000 tarn-0.6.0/tarn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-08 11:40:19.000000 tarn-0.6.0/tarn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-08 11:40:19.000000 tarn-0.6.0/tarn.egg-info/top_level.txt
```

### Comparing `tarn-0.5.1/LICENSE` & `tarn-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tarn-0.5.1/PKG-INFO` & `tarn-0.6.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: tarn
-Version: 0.5.1
+Version: 0.6.0
 Summary: A hashmap-based storage on local and remote disks
 Home-page: https://github.com/neuro-ml/tarn
+Author: Max
+Author-email: max@ira-labs.com
 License: UNKNOWN
-Download-URL: https://github.com/neuro-ml/tarn/archive/v0.5.1.tar.gz
+Download-URL: https://github.com/neuro-ml/tarn/archive/v0.6.0.tar.gz
 Keywords: storage,cache,invalidation
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `tarn-0.5.1/README.md` & `tarn-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `tarn-0.5.1/pyproject.toml` & `tarn-0.6.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 dynamic = ['version', 'dependencies']
 description = 'A hashmap-based storage on local and remote disks'
 readme = 'README.md'
 requires-python = '>=3.6'
 license = { file = 'LICENSE' }
 keywords = ['storage', 'cache', 'invalidation']
 authors = [
-    { name = 'Max', email = 'maxs987@gmail.com' }
+    { name = 'Max', email = 'max@ira-labs.com' }
 ]
 classifiers = [
     'Development Status :: 3 - Alpha',
     'License :: OSI Approved :: Apache Software License',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.6',
     'Programming Language :: Python :: 3.7',
```

### Comparing `tarn-0.5.1/setup.py` & `tarn-0.6.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 version = runpy.run_path(root / name / '__version__.py')['__version__']
 
 setup(
     name=name,
     packages=find_packages(include=(name,)),
     include_package_data=True,
     version=version,
+    author='Max',
+    author_email='max@ira-labs.com',
     description='A hashmap-based storage on local and remote disks',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/neuro-ml/tarn',
     download_url='https://github.com/neuro-ml/tarn/archive/v%s.tar.gz' % version,
     keywords=['storage', 'cache', 'invalidation'],
     classifiers=classifiers,
```

### Comparing `tarn-0.5.1/tarn/cache/storage.py` & `tarn-0.6.0/tarn/cache/storage.py`

 * *Files identical despite different names*

### Comparing `tarn-0.5.1/tarn/compat.py` & `tarn-0.6.0/tarn/compat.py`

 * *Files identical despite different names*

### Comparing `tarn-0.5.1/tarn/config.py` & `tarn-0.6.0/tarn/config.py`

 * *Files identical despite different names*

### Comparing `tarn-0.5.1/tarn/digest.py` & `tarn-0.6.0/tarn/digest.py`

 * *Files identical despite different names*

### Comparing `tarn-0.5.1/tarn/interface.py` & `tarn-0.6.0/tarn/interface.py`

 * *Files identical despite different names*

### Comparing `tarn-0.5.1/tarn/local/storage.py` & `tarn-0.6.0/tarn/local/storage.py`

 * *Files identical despite different names*

### Comparing `tarn-0.5.1/tarn/location/disk_dict.py` & `tarn-0.6.0/tarn/location/disk_dict.py`

 * *Files identical despite different names*

### Comparing `tarn-0.5.1/tarn/location/fanout.py` & `tarn-0.6.0/tarn/location/fanout.py`

 * *Files identical despite different names*

### Comparing `tarn-0.5.1/tarn/location/levels.py` & `tarn-0.6.0/tarn/location/levels.py`

 * *Files identical despite different names*

### Comparing `tarn-0.5.1/tarn/location/nginx.py` & `tarn-0.6.0/tarn/location/nginx.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,22 +38,23 @@
     def _read_single(self, key: Key) -> ContextManager[MaybeValue]:
         if self.levels is None:
             yield None
             return
 
         relative = key_to_relative(key, self.levels)
         with requests.get(urljoin(self.url, str(relative)), stream=True) as request:
-            if not request.ok:
+            if request.status_code == 301:
                 # TODO: this is probably an old format directory
                 with requests.get(urljoin(self.url, str(relative / 'data')), stream=True) as req:
                     if req.ok:
                         with req.raw as raw:
                             yield raw
                             return
 
+            if not request.ok:
                 yield None
                 return
 
             with request.raw as raw:
                 yield raw
 
     def _get_config(self):
```

### Comparing `tarn-0.5.1/tarn/location/scp.py` & `tarn-0.6.0/tarn/location/scp.py`

 * *Files identical despite different names*

### Comparing `tarn-0.5.1/tarn/pickler/compat.py` & `tarn-0.6.0/tarn/pickler/compat.py`

 * *Files identical despite different names*

### Comparing `tarn-0.5.1/tarn/pickler/interface.py` & `tarn-0.6.0/tarn/pickler/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,20 +55,24 @@
 
     def __init__(self, file, protocol=None, version=None):
         if version is None:
             version = LATEST_VERSION
 
         super().__init__(file, protocol=protocol)
         self.version = version
+        self._interning = {}
         self.dispatch_table = {
             types.CodeType: self.reduce_code,
             property: self.reduce_property,
         }
 
     def save(self, obj, *args, **kwargs):
+        if isinstance(obj, str):
+            obj = self._interning.setdefault(obj, obj)
+
         try:
             return super().save(obj, *args, **kwargs)
         except PickleError as e:
             raise PickleError(str(e)) from None
         except BaseException as e:
             raise PickleError(f'Exception "{e.__class__.__name__}: {e}" '
                               f'while pickling object {obj}') from None
```

### Comparing `tarn-0.5.1/tarn/pool/hash_key.py` & `tarn-0.6.0/tarn/pool/hash_key.py`

 * *Files identical despite different names*

### Comparing `tarn-0.5.1/tarn/pool/pickle_key.py` & `tarn-0.6.0/tarn/pool/pickle_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,17 +77,16 @@
                     continue
 
                 relative = str(file.relative_to(temp_folder))
                 assert relative not in mapping
                 mapping[relative] = self.storage.write(file, labels=labels).hex()
 
         # we want a reproducible mapping each time
-        mapping = {k: mapping[k] for k in sorted(mapping)}
         logger.info('Saving to index %s', digest)
-        with self.index.write(digest, BytesIO(json.dumps(mapping).encode()), labels=None) as written:
+        with self.index.write(digest, BytesIO(json.dumps(mapping, sort_keys=True).encode()), labels=None) as written:
             if written is None:
                 if error:
                     raise WriteError('The index could not be written to any storage')
                 return None
 
         return digest
 
@@ -98,17 +97,16 @@
 
             with _unpack_mapping(index) as folder:
                 try:
                     return self.serializer.load(folder, self.storage), True
                 # either the data is corrupted or missing
                 except (DeserializationError, ReadError) as e:
                     raise StorageCorruption from e
-
-                except SerializerError:
-                    raise
+                except SerializerError as e:
+                    raise SerializerError(f'Could not deserialize the data from key {digest.hex()}') from e
                 except Exception as e:
                     raise RuntimeError(f'An error occurred while loading the cache for "{digest.hex()}"') from e
 
         return None, False
 
     def _read(self, key: _PreparedKey):
         digest = key.digest
```

### Comparing `tarn-0.5.1/tarn/serializers.py` & `tarn-0.6.0/tarn/serializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
         raise SerializerError(f'No serializer was able to load from {folder}.')
 
 
 class JsonSerializer(Serializer):
     def save(self, value, folder: Path):
         try:
-            value = json.dumps(value)
+            value = json.dumps(value, sort_keys=True)
         except TypeError as e:
             raise SerializerError from e
 
         with open(folder / 'value.json', 'w') as file:
             file.write(value)
 
     def load(self, folder: Path, storage: HashKeyStorage):
@@ -176,15 +176,15 @@
             # remove the partially saved object
             for sub_folder in folder.iterdir():
                 rmtree(sub_folder)
 
             raise
 
         with open(folder / self.keys_filename, 'w+') as f:
-            json.dump(keys_to_folder, f)
+            json.dump(keys_to_folder, f, sort_keys=True)
 
     def load(self, folder: Path, storage: HashKeyStorage):
         keys = folder / self.keys_filename
         if not keys.exists():
             raise SerializerError
 
         def loader(x):
```

### Comparing `tarn-0.5.1/tarn/tools/labels.py` & `tarn-0.6.0/tarn/tools/labels.py`

 * *Files identical despite different names*

### Comparing `tarn-0.5.1/tarn/tools/locker.py` & `tarn-0.6.0/tarn/tools/locker.py`

 * *Files identical despite different names*

### Comparing `tarn-0.5.1/tarn/tools/size.py` & `tarn-0.6.0/tarn/tools/size.py`

 * *Files identical despite different names*

### Comparing `tarn-0.5.1/tarn/tools/usage.py` & `tarn-0.6.0/tarn/tools/usage.py`

 * *Files identical despite different names*

### Comparing `tarn-0.5.1/tarn/utils.py` & `tarn-0.6.0/tarn/utils.py`

 * *Files identical despite different names*

### Comparing `tarn-0.5.1/tarn.egg-info/PKG-INFO` & `tarn-0.6.0/tarn.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: tarn
-Version: 0.5.1
+Version: 0.6.0
 Summary: A hashmap-based storage on local and remote disks
 Home-page: https://github.com/neuro-ml/tarn
+Author: Max
+Author-email: max@ira-labs.com
 License: UNKNOWN
-Download-URL: https://github.com/neuro-ml/tarn/archive/v0.5.1.tar.gz
+Download-URL: https://github.com/neuro-ml/tarn/archive/v0.6.0.tar.gz
 Keywords: storage,cache,invalidation
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `tarn-0.5.1/tarn.egg-info/SOURCES.txt` & `tarn-0.6.0/tarn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

