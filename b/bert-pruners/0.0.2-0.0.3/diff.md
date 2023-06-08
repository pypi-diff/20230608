# Comparing `tmp/bert_pruners-0.0.2.tar.gz` & `tmp/bert_pruners-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bert_pruners-0.0.2.tar", last modified: Tue Jun  6 16:00:24 2023, max compression
+gzip compressed data, was "bert_pruners-0.0.3.tar", last modified: Thu Jun  8 08:10:09 2023, max compression
```

## Comparing `bert_pruners-0.0.2.tar` & `bert_pruners-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-06-06 16:00:24.445092 bert_pruners-0.0.2/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       43 2023-06-06 14:47:28.000000 bert_pruners-0.0.2/MANIFEST.in
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      350 2023-06-06 16:00:24.445092 bert_pruners-0.0.2/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       86 2023-06-06 15:01:38.000000 bert_pruners-0.0.2/README.md
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-06-06 16:00:24.441092 bert_pruners-0.0.2/bert_pruners/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-06-06 14:47:28.000000 bert_pruners-0.0.2/bert_pruners/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1776 2023-06-06 15:29:51.000000 bert_pruners-0.0.2/bert_pruners/bert_pruner.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      675 2023-06-06 15:59:59.000000 bert_pruners-0.0.2/bert_pruners/main.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-06-06 16:00:24.445092 bert_pruners-0.0.2/bert_pruners.egg-info/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      350 2023-06-06 16:00:24.000000 bert_pruners-0.0.2/bert_pruners.egg-info/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      322 2023-06-06 16:00:24.000000 bert_pruners-0.0.2/bert_pruners.egg-info/SOURCES.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-06-06 16:00:24.000000 bert_pruners-0.0.2/bert_pruners.egg-info/dependency_links.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       54 2023-06-06 16:00:24.000000 bert_pruners-0.0.2/bert_pruners.egg-info/entry_points.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       24 2023-06-06 16:00:24.000000 bert_pruners-0.0.2/bert_pruners.egg-info/requires.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       13 2023-06-06 16:00:24.000000 bert_pruners-0.0.2/bert_pruners.egg-info/top_level.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2023-06-06 16:00:24.445092 bert_pruners-0.0.2/setup.cfg
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      675 2023-06-06 16:00:21.000000 bert_pruners-0.0.2/setup.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-06-08 08:10:09.379806 bert_pruners-0.0.3/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       43 2023-06-08 08:09:51.000000 bert_pruners-0.0.3/MANIFEST.in
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      350 2023-06-08 08:10:09.375806 bert_pruners-0.0.3/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       86 2023-06-08 08:09:51.000000 bert_pruners-0.0.3/README.md
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-06-08 08:10:09.375806 bert_pruners-0.0.3/bert_pruners/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-06-08 07:52:13.000000 bert_pruners-0.0.3/bert_pruners/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1776 2023-06-08 07:52:13.000000 bert_pruners-0.0.3/bert_pruners/bert_pruner.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      688 2023-06-08 08:08:20.000000 bert_pruners-0.0.3/bert_pruners/main.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-06-08 08:10:09.375806 bert_pruners-0.0.3/bert_pruners.egg-info/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      350 2023-06-08 08:10:09.000000 bert_pruners-0.0.3/bert_pruners.egg-info/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      322 2023-06-08 08:10:09.000000 bert_pruners-0.0.3/bert_pruners.egg-info/SOURCES.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-06-08 08:10:09.000000 bert_pruners-0.0.3/bert_pruners.egg-info/dependency_links.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       54 2023-06-08 08:10:09.000000 bert_pruners-0.0.3/bert_pruners.egg-info/entry_points.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       24 2023-06-08 08:10:09.000000 bert_pruners-0.0.3/bert_pruners.egg-info/requires.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       13 2023-06-08 08:10:09.000000 bert_pruners-0.0.3/bert_pruners.egg-info/top_level.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2023-06-08 08:10:09.379806 bert_pruners-0.0.3/setup.cfg
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      675 2023-06-08 08:10:04.000000 bert_pruners-0.0.3/setup.py
```

### Comparing `bert_pruners-0.0.2/bert_pruners/bert_pruner.py` & `bert_pruners-0.0.3/bert_pruners/bert_pruner.py`

 * *Files identical despite different names*

### Comparing `bert_pruners-0.0.2/bert_pruners/main.py` & `bert_pruners-0.0.3/bert_pruners/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import argparse
 from .bert_pruner import BertPruner
 
 def main():
     parser = argparse.ArgumentParser(description='BERT pruner')
     parser.add_argument('--model_name', default='xihajun/krai-mlperf-inference-v3.0-bert-pytorch-fp32-squad-v1.1', type=str, help='Path to save the pruned model')
     parser.add_argument('--saved_dir', type=str, help='Path to save the pruned model')
-    parser.add_argument('--sparsity', type=float, help='Desired sparsity of the pruned model')
+    parser.add_argument('--sparsity', type=float, default=0.5, help='Desired sparsity of the pruned model')
     args = parser.parse_args()
 
     pruner = BertPruner(model_name=args.model_name, saved_dir=args.saved_dir, sparsity=args.sparsity)
     pruner.prune_and_save()
 
 if __name__ == "__main__":
     main()
```

### Comparing `bert_pruners-0.0.2/setup.py` & `bert_pruners-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="bert_pruners",
-    version="0.0.2",
+    version="0.0.3",
     author="xihajun",
     author_email="junfan@krai.ai",
     description="Pruning BERT models",
     url="https://github.com/xihajun/bert_pruners",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
```

