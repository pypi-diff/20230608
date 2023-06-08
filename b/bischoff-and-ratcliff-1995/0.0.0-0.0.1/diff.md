# Comparing `tmp/bischoff_and_ratcliff_1995-0.0.0.tar.gz` & `tmp/bischoff_and_ratcliff_1995-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bischoff_and_ratcliff_1995-0.0.0.tar", last modified: Thu Jun  8 18:56:25 2023, max compression
+gzip compressed data, was "bischoff_and_ratcliff_1995-0.0.1.tar", last modified: Thu Jun  8 19:28:46 2023, max compression
```

## Comparing `bischoff_and_ratcliff_1995-0.0.0.tar` & `bischoff_and_ratcliff_1995-0.0.1.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 unicamp   (1001) unicamp   (1001)        0 2023-06-08 18:56:25.659184 bischoff_and_ratcliff_1995-0.0.0/
--rw-r--r--   0 unicamp   (1001) unicamp   (1001)     1070 2023-06-08 14:26:14.000000 bischoff_and_ratcliff_1995-0.0.0/LICENSE
--rw-r--r--   0 unicamp   (1001) unicamp   (1001)      582 2023-06-08 18:56:25.659184 bischoff_and_ratcliff_1995-0.0.0/PKG-INFO
--rw-r--r--   0 unicamp   (1001) unicamp   (1001)      734 2023-06-08 18:32:24.000000 bischoff_and_ratcliff_1995-0.0.0/README.md
-drwxr-xr-x   0 unicamp   (1001) unicamp   (1001)        0 2023-06-08 18:56:25.658184 bischoff_and_ratcliff_1995-0.0.0/bischoff_and_ratcliff_1995/
--rw-r--r--   0 unicamp   (1001) unicamp   (1001)     3038 2023-06-08 18:32:24.000000 bischoff_and_ratcliff_1995-0.0.0/bischoff_and_ratcliff_1995/Instance.py
--rw-r--r--   0 unicamp   (1001) unicamp   (1001)      448 2023-06-08 18:32:24.000000 bischoff_and_ratcliff_1995-0.0.0/bischoff_and_ratcliff_1995/Random.py
--rw-r--r--   0 unicamp   (1001) unicamp   (1001)       58 2023-06-08 18:32:24.000000 bischoff_and_ratcliff_1995-0.0.0/bischoff_and_ratcliff_1995/__init__.py
-drwxr-xr-x   0 unicamp   (1001) unicamp   (1001)        0 2023-06-08 18:56:25.659184 bischoff_and_ratcliff_1995-0.0.0/bischoff_and_ratcliff_1995.egg-info/
--rw-r--r--   0 unicamp   (1001) unicamp   (1001)      582 2023-06-08 18:56:25.000000 bischoff_and_ratcliff_1995-0.0.0/bischoff_and_ratcliff_1995.egg-info/PKG-INFO
--rw-r--r--   0 unicamp   (1001) unicamp   (1001)      447 2023-06-08 18:56:25.000000 bischoff_and_ratcliff_1995-0.0.0/bischoff_and_ratcliff_1995.egg-info/SOURCES.txt
--rw-r--r--   0 unicamp   (1001) unicamp   (1001)        1 2023-06-08 18:56:25.000000 bischoff_and_ratcliff_1995-0.0.0/bischoff_and_ratcliff_1995.egg-info/dependency_links.txt
--rw-r--r--   0 unicamp   (1001) unicamp   (1001)        7 2023-06-08 18:56:25.000000 bischoff_and_ratcliff_1995-0.0.0/bischoff_and_ratcliff_1995.egg-info/requires.txt
--rw-r--r--   0 unicamp   (1001) unicamp   (1001)       27 2023-06-08 18:56:25.000000 bischoff_and_ratcliff_1995-0.0.0/bischoff_and_ratcliff_1995.egg-info/top_level.txt
--rw-r--r--   0 unicamp   (1001) unicamp   (1001)      116 2023-06-08 18:44:53.000000 bischoff_and_ratcliff_1995-0.0.0/pyproject.toml
--rw-r--r--   0 unicamp   (1001) unicamp   (1001)       38 2023-06-08 18:56:25.659184 bischoff_and_ratcliff_1995-0.0.0/setup.cfg
--rw-r--r--   0 unicamp   (1001) unicamp   (1001)      767 2023-06-08 18:56:18.000000 bischoff_and_ratcliff_1995-0.0.0/setup.py
-drwxr-xr-x   0 unicamp   (1001) unicamp   (1001)        0 2023-06-08 18:56:25.659184 bischoff_and_ratcliff_1995-0.0.0/test/
--rw-r--r--   0 unicamp   (1001) unicamp   (1001)     2119 2023-06-08 18:32:24.000000 bischoff_and_ratcliff_1995-0.0.0/test/test_Instance.py
--rw-r--r--   0 unicamp   (1001) unicamp   (1001)      569 2023-06-08 18:32:24.000000 bischoff_and_ratcliff_1995-0.0.0/test/test_Random.py
+drwxr-xr-x   0 unicamp   (1001) unicamp   (1001)        0 2023-06-08 19:28:46.028236 bischoff_and_ratcliff_1995-0.0.1/
+-rw-r--r--   0 unicamp   (1001) unicamp   (1001)     1070 2023-06-08 14:26:14.000000 bischoff_and_ratcliff_1995-0.0.1/LICENSE
+-rw-r--r--   0 unicamp   (1001) unicamp   (1001)      582 2023-06-08 19:28:46.027236 bischoff_and_ratcliff_1995-0.0.1/PKG-INFO
+-rw-r--r--   0 unicamp   (1001) unicamp   (1001)      733 2023-06-08 19:27:04.000000 bischoff_and_ratcliff_1995-0.0.1/README.md
+drwxr-xr-x   0 unicamp   (1001) unicamp   (1001)        0 2023-06-08 19:28:46.026236 bischoff_and_ratcliff_1995-0.0.1/bin/
+-rwxr-xr-x   0 unicamp   (1001) unicamp   (1001)     2433 2023-06-08 19:25:19.000000 bischoff_and_ratcliff_1995-0.0.1/bin/generate_all_instances
+drwxr-xr-x   0 unicamp   (1001) unicamp   (1001)        0 2023-06-08 19:28:46.026236 bischoff_and_ratcliff_1995-0.0.1/bischoff_and_ratcliff_1995/
+-rw-r--r--   0 unicamp   (1001) unicamp   (1001)     3038 2023-06-08 18:32:24.000000 bischoff_and_ratcliff_1995-0.0.1/bischoff_and_ratcliff_1995/Instance.py
+-rw-r--r--   0 unicamp   (1001) unicamp   (1001)      448 2023-06-08 18:32:24.000000 bischoff_and_ratcliff_1995-0.0.1/bischoff_and_ratcliff_1995/Random.py
+-rw-r--r--   0 unicamp   (1001) unicamp   (1001)       58 2023-06-08 18:32:24.000000 bischoff_and_ratcliff_1995-0.0.1/bischoff_and_ratcliff_1995/__init__.py
+drwxr-xr-x   0 unicamp   (1001) unicamp   (1001)        0 2023-06-08 19:28:46.027236 bischoff_and_ratcliff_1995-0.0.1/bischoff_and_ratcliff_1995.egg-info/
+-rw-r--r--   0 unicamp   (1001) unicamp   (1001)      582 2023-06-08 19:28:46.000000 bischoff_and_ratcliff_1995-0.0.1/bischoff_and_ratcliff_1995.egg-info/PKG-INFO
+-rw-r--r--   0 unicamp   (1001) unicamp   (1001)      474 2023-06-08 19:28:46.000000 bischoff_and_ratcliff_1995-0.0.1/bischoff_and_ratcliff_1995.egg-info/SOURCES.txt
+-rw-r--r--   0 unicamp   (1001) unicamp   (1001)        1 2023-06-08 19:28:46.000000 bischoff_and_ratcliff_1995-0.0.1/bischoff_and_ratcliff_1995.egg-info/dependency_links.txt
+-rw-r--r--   0 unicamp   (1001) unicamp   (1001)        7 2023-06-08 19:28:46.000000 bischoff_and_ratcliff_1995-0.0.1/bischoff_and_ratcliff_1995.egg-info/requires.txt
+-rw-r--r--   0 unicamp   (1001) unicamp   (1001)       27 2023-06-08 19:28:46.000000 bischoff_and_ratcliff_1995-0.0.1/bischoff_and_ratcliff_1995.egg-info/top_level.txt
+-rw-r--r--   0 unicamp   (1001) unicamp   (1001)      116 2023-06-08 19:27:04.000000 bischoff_and_ratcliff_1995-0.0.1/pyproject.toml
+-rw-r--r--   0 unicamp   (1001) unicamp   (1001)       38 2023-06-08 19:28:46.028236 bischoff_and_ratcliff_1995-0.0.1/setup.cfg
+-rw-r--r--   0 unicamp   (1001) unicamp   (1001)      801 2023-06-08 19:27:04.000000 bischoff_and_ratcliff_1995-0.0.1/setup.py
+drwxr-xr-x   0 unicamp   (1001) unicamp   (1001)        0 2023-06-08 19:28:46.027236 bischoff_and_ratcliff_1995-0.0.1/test/
+-rw-r--r--   0 unicamp   (1001) unicamp   (1001)     2119 2023-06-08 18:32:24.000000 bischoff_and_ratcliff_1995-0.0.1/test/test_Instance.py
+-rw-r--r--   0 unicamp   (1001) unicamp   (1001)      569 2023-06-08 18:32:24.000000 bischoff_and_ratcliff_1995-0.0.1/test/test_Random.py
```

### Comparing `bischoff_and_ratcliff_1995-0.0.0/LICENSE` & `bischoff_and_ratcliff_1995-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bischoff_and_ratcliff_1995-0.0.0/PKG-INFO` & `bischoff_and_ratcliff_1995-0.0.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bischoff_and_ratcliff_1995
-Version: 0.0.0
+Version: 0.0.1
 Summary: Instance generator, as described in the paper of Bischoff and Ratcliff (1995)
 Home-page: https://github.com/lucasguesserts/bischoff-and-ratcliff-1995
 Author: Lucas Guesser
 Author-email: lucasguesserts@gmail.com
 Keywords: container loading problem,knapsack problem,single large object placement problem (slopp),packing problem
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bischoff_and_ratcliff_1995-0.0.0/README.md` & `bischoff_and_ratcliff_1995-0.0.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -7,14 +7,14 @@
 ```sh
 $ pip install -e .
 (...) pip install log stuff (...)
 $ pytest
 === test session starts ===
 (...) pytest logs (...)
 === X passed in Y.ZZ s ===
-$ ./bin/generate_all_instances
-instances written into 'instances.json'
+$ generate_all_instances
+instances written into the directory 'data/'
 ```
 
 ## File Format
 
 The [file format](https://github.com/lucasguesserts/packing-visualizer/tree/trunk/src/file_format/input) is based on the specifications in the [packing-visualizer project](https://github.com/lucasguesserts/packing-visualizer/).
```

### Comparing `bischoff_and_ratcliff_1995-0.0.0/bischoff_and_ratcliff_1995/Instance.py` & `bischoff_and_ratcliff_1995-0.0.1/bischoff_and_ratcliff_1995/Instance.py`

 * *Files identical despite different names*

### Comparing `bischoff_and_ratcliff_1995-0.0.0/bischoff_and_ratcliff_1995.egg-info/PKG-INFO` & `bischoff_and_ratcliff_1995-0.0.1/bischoff_and_ratcliff_1995.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bischoff-and-ratcliff-1995
-Version: 0.0.0
+Version: 0.0.1
 Summary: Instance generator, as described in the paper of Bischoff and Ratcliff (1995)
 Home-page: https://github.com/lucasguesserts/bischoff-and-ratcliff-1995
 Author: Lucas Guesser
 Author-email: lucasguesserts@gmail.com
 Keywords: container loading problem,knapsack problem,single large object placement problem (slopp),packing problem
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bischoff_and_ratcliff_1995-0.0.0/setup.py` & `bischoff_and_ratcliff_1995-0.0.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from setuptools import setup
 
 setup(
     # Metadata
-    name='bischoff_and_ratcliff_1995',
-    version='0.0.0',
-    description='Instance generator, as described in the paper of Bischoff and Ratcliff (1995)',
-    url='https://github.com/lucasguesserts/bischoff-and-ratcliff-1995',
-    author='Lucas Guesser',
-    author_email='lucasguesserts@gmail.com',
+    name="bischoff_and_ratcliff_1995",
+    version="0.0.1",
+    description="Instance generator, as described in the paper of Bischoff and Ratcliff (1995)",
+    url="https://github.com/lucasguesserts/bischoff-and-ratcliff-1995",
+    author="Lucas Guesser",
+    author_email="lucasguesserts@gmail.com",
     classifiers=[
-        'Natural Language :: English',
-        'Programming Language :: Python :: 3',
-        'Topic :: Scientific/Engineering',
+        "Natural Language :: English",
+        "Programming Language :: Python :: 3",
+        "Topic :: Scientific/Engineering",
     ],
-	keywords=[
-        'container loading problem',
-        'knapsack problem',
-        'single large object placement problem (slopp)',
-        'packing problem'
+    keywords=[
+        "container loading problem",
+        "knapsack problem",
+        "single large object placement problem (slopp)",
+        "packing problem",
     ],
     # Options
-    install_requires=[
-        'pytest'
-    ],
-    python_requires='>=3.0',
+    install_requires=["pytest"],
+    python_requires=">=3.0",
+    scripts=["bin/generate_all_instances"],
 )
```

### Comparing `bischoff_and_ratcliff_1995-0.0.0/test/test_Instance.py` & `bischoff_and_ratcliff_1995-0.0.1/test/test_Instance.py`

 * *Files identical despite different names*

### Comparing `bischoff_and_ratcliff_1995-0.0.0/test/test_Random.py` & `bischoff_and_ratcliff_1995-0.0.1/test/test_Random.py`

 * *Files identical despite different names*

