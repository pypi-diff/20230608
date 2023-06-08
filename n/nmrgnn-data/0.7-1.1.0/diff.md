# Comparing `tmp/nmrgnn-data-0.7.tar.gz` & `tmp/nmrgnn-data-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmrgnn-data-0.7.tar", last modified: Tue Aug 31 03:04:49 2021, max compression
+gzip compressed data, was "nmrgnn-data-1.1.0.tar", last modified: Thu Jun  8 20:00:53 2023, max compression
```

## Comparing `nmrgnn-data-0.7.tar` & `nmrgnn-data-1.1.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-31 03:04:49.024978 nmrgnn-data-0.7/
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2021-08-31 03:02:19.000000 nmrgnn-data-0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3179 2021-08-31 03:04:49.024978 nmrgnn-data-0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2561 2021-08-31 03:02:19.000000 nmrgnn-data-0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-31 03:04:49.020978 nmrgnn-data-0.7/nmrdata/
--rw-r--r--   0 runner    (1001) docker     (121)       82 2021-08-31 03:02:19.000000 nmrgnn-data-0.7/nmrdata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-31 03:04:49.020978 nmrgnn-data-0.7/nmrdata/data/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-31 03:02:19.000000 nmrgnn-data-0.7/nmrdata/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8101 2021-08-31 03:02:19.000000 nmrgnn-data-0.7/nmrdata/data/embeddings.pb
--rw-r--r--   0 runner    (1001) docker     (121)      557 2021-08-31 03:02:19.000000 nmrgnn-data-0.7/nmrdata/data/standards.pb
--rw-r--r--   0 runner    (1001) docker     (121)    14058 2021-08-31 03:02:19.000000 nmrgnn-data-0.7/nmrdata/loading.py
--rw-r--r--   0 runner    (1001) docker     (121)      335 2021-08-31 03:02:19.000000 nmrgnn-data-0.7/nmrdata/main.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-31 03:04:49.024978 nmrgnn-data-0.7/nmrdata/parse/
--rw-r--r--   0 runner    (1001) docker     (121)       28 2021-08-31 03:02:19.000000 nmrgnn-data-0.7/nmrdata/parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1851 2021-08-31 03:02:19.000000 nmrgnn-data-0.7/nmrdata/parse/add_dssp.py
--rw-r--r--   0 runner    (1001) docker     (121)     1817 2021-08-31 03:02:19.000000 nmrgnn-data-0.7/nmrdata/parse/add_weights.py
--rw-r--r--   0 runner    (1001) docker     (121)     1752 2021-08-31 03:02:19.000000 nmrgnn-data-0.7/nmrdata/parse/label_standardize.py
--rw-r--r--   0 runner    (1001) docker     (121)     1271 2021-08-31 03:02:19.000000 nmrgnn-data-0.7/nmrdata/parse/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     6808 2021-08-31 03:02:19.000000 nmrgnn-data-0.7/nmrdata/parse/metabolite_tfrecords.py
--rw-r--r--   0 runner    (1001) docker     (121)      524 2021-08-31 03:02:19.000000 nmrgnn-data-0.7/nmrdata/parse/prepare_shiftx_records.py
--rw-r--r--   0 runner    (1001) docker     (121)    19436 2021-08-31 03:02:19.000000 nmrgnn-data-0.7/nmrdata/parse/protein_tfrecords.py
--rw-r--r--   0 runner    (1001) docker     (121)     3509 2021-08-31 03:02:19.000000 nmrgnn-data-0.7/nmrdata/parse/shiftml_tfrecords.py
--rw-r--r--   0 runner    (1001) docker     (121)    11502 2021-08-31 03:02:19.000000 nmrgnn-data-0.7/nmrdata/validation.py
--rw-r--r--   0 runner    (1001) docker     (121)       20 2021-08-31 03:02:19.000000 nmrgnn-data-0.7/nmrdata/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-31 03:04:49.024978 nmrgnn-data-0.7/nmrgnn_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3179 2021-08-31 03:04:48.000000 nmrgnn-data-0.7/nmrgnn_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      728 2021-08-31 03:04:49.000000 nmrgnn-data-0.7/nmrgnn_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-31 03:04:48.000000 nmrgnn-data-0.7/nmrgnn_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      121 2021-08-31 03:04:48.000000 nmrgnn-data-0.7/nmrgnn_data.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      104 2021-08-31 03:04:48.000000 nmrgnn-data-0.7/nmrgnn_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2021-08-31 03:04:48.000000 nmrgnn-data-0.7/nmrgnn_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-31 03:04:48.000000 nmrgnn-data-0.7/nmrgnn_data.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-08-31 03:04:49.024978 nmrgnn-data-0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1453 2021-08-31 03:02:19.000000 nmrgnn-data-0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:00:53.737123 nmrgnn-data-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-08 19:59:37.000000 nmrgnn-data-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-06-08 20:00:53.737123 nmrgnn-data-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-06-08 19:59:37.000000 nmrgnn-data-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:00:53.733123 nmrgnn-data-1.1.0/nmrdata/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-08 19:59:37.000000 nmrgnn-data-1.1.0/nmrdata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:00:53.733123 nmrgnn-data-1.1.0/nmrdata/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 19:59:37.000000 nmrgnn-data-1.1.0/nmrdata/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8274 2023-06-08 19:59:37.000000 nmrgnn-data-1.1.0/nmrdata/data/embeddings.pb
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-08 19:59:37.000000 nmrgnn-data-1.1.0/nmrdata/data/standards.pb
+-rw-r--r--   0 runner    (1001) docker     (123)    14659 2023-06-08 19:59:37.000000 nmrgnn-data-1.1.0/nmrdata/loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-08 19:59:37.000000 nmrgnn-data-1.1.0/nmrdata/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:00:53.733123 nmrgnn-data-1.1.0/nmrdata/parse/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-08 19:59:37.000000 nmrgnn-data-1.1.0/nmrdata/parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-08 19:59:37.000000 nmrgnn-data-1.1.0/nmrdata/parse/add_dssp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-08 19:59:37.000000 nmrgnn-data-1.1.0/nmrdata/parse/add_weights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-06-08 19:59:37.000000 nmrgnn-data-1.1.0/nmrdata/parse/cascade_tfrecords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-08 19:59:37.000000 nmrgnn-data-1.1.0/nmrdata/parse/label_standardize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-08 19:59:37.000000 nmrgnn-data-1.1.0/nmrdata/parse/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-06-08 19:59:37.000000 nmrgnn-data-1.1.0/nmrdata/parse/metabolite_tfrecords.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-08 19:59:37.000000 nmrgnn-data-1.1.0/nmrdata/parse/prepare_shiftx_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19428 2023-06-08 19:59:37.000000 nmrgnn-data-1.1.0/nmrdata/parse/protein_tfrecords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-06-08 19:59:37.000000 nmrgnn-data-1.1.0/nmrdata/parse/shiftml_tfrecords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-06-08 19:59:37.000000 nmrgnn-data-1.1.0/nmrdata/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-08 19:59:37.000000 nmrgnn-data-1.1.0/nmrdata/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:00:53.737123 nmrgnn-data-1.1.0/nmrgnn_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-06-08 20:00:53.000000 nmrgnn-data-1.1.0/nmrgnn_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-08 20:00:53.000000 nmrgnn-data-1.1.0/nmrgnn_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 20:00:53.000000 nmrgnn-data-1.1.0/nmrgnn_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-08 20:00:53.000000 nmrgnn-data-1.1.0/nmrgnn_data.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-08 20:00:53.000000 nmrgnn-data-1.1.0/nmrgnn_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-08 20:00:53.000000 nmrgnn-data-1.1.0/nmrgnn_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 19:59:46.000000 nmrgnn-data-1.1.0/nmrgnn_data.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 20:00:53.737123 nmrgnn-data-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-08 19:59:37.000000 nmrgnn-data-1.1.0/setup.py
```

### Comparing `nmrgnn-data-0.7/LICENSE` & `nmrgnn-data-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nmrgnn-data-0.7/PKG-INFO` & `nmrgnn-data-1.1.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,58 @@
-Metadata-Version: 2.1
-Name: nmrgnn-data
-Version: 0.7
-Summary: Chemical shift prediction dataset
-Home-page: https://github.com/ur-whitelab/nmrdata
-Author: Ziyue Yang, Andrew White
-Author-email: andrew.white@rochester.edu
-License: MIT
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Description-Content-Type: text/markdown
-Provides-Extra: parse
-License-File: LICENSE
-
 # Data for NMR GNN
 
 This contains the parsing scripts and data used for our [GNN chemical shift predictor model](https://github.com/ur-whitelab/nmrgnn).
 
 ## Install
 
 ```sh
 pip install nmrgnn-data
 ```
 
+## Working in Python
+
+Here's an example of how to load and work with data in python. The records
+are loaded as a tensorflow dataset ([read more here](https://www.tensorflow.org/api_docs/python/tf/data/Dataset)), but can be used in a for loop as shown below.
+
+```py
+import nmrdata
+dataset = nmrdata.load_records('data/metabolite-records.tfrecord')
+for record in dataset:
+    # get single record
+    break
+print(record.keys())
+```
+output:
+```
+dict_keys(['natoms', 'nneigh', 'features', 'nlist', 'positions', 'peaks', 'mask', 'name', 'class', 'index'])
+```
+
+Access positions as a numpy array
+```py
+record['positions'].numpy()
+```
+output:
+```
+array([[ 0.83740795,  0.09760247,  0.2959486 ],
+       [-0.562893  ,  0.00262405, -0.00434441],
+       [-1.0725924 , -0.37873718,  0.9061929 ],
+       [-0.75536764, -0.72710234, -0.8159687 ],
+       [-1.0367495 ,  0.9557108 , -0.27988592],
+       [ 1.2855262 , -0.8334997 ,  0.10487328],
+       [ 1.3046683 ,  0.8834019 , -0.20681578]], dtype=float32)
+```
+Get chemical shifts
+```py
+record['peaks'].numpy()
+```
+```
+array([0.  , 0.  , 2.59, 2.59, 2.59, 0.  , 0.  ], dtype=float32)
+```
+
+
 ## Numpy Error
 
 If you see this error:
 
 ```py
 ValueError: numpy.ndarray size changed, may indicate binary incompatibility. Expected 88 from C header, got 80 from PyObject
 ```
@@ -39,15 +62,15 @@
 pip uninstall -y numpy && pip install numpy
 ```
 
 ## Parsing Scripts
 To install with the parsing functionality, use this
 
 ```sh
-conda install -c omnia -c conda-forge rdkit openmm numpy==1.18.5
+conda install -c omnia openmm
 pip install nmrgnn-data[parse]
 ```
 
 ## Working with Data
 
 All commands below can have additional information printed using the `--help` argument.
 
@@ -93,15 +116,15 @@
 
 ```sh
 nmrdata write-peak-labels test-structure-shift-data.tfrecord  test-structure-shift-record-info.txt labels.txt
 ```
 
 ## Making New Data
 
-See commands `parse-shiftml`, `parse-metabolites`, `parse-shiftx` which are parsers for various databases.
+See commands `nmrparse shiftml`, `nmrparse metabolites`, `nmrparse shiftx` which are parsers for various databases.
 
 ### From RefDB Files
 
 This requires a pickled python object called `data.pb` to be in the directory. It is
 a list of `dict`s containing `pdb_file` (path to PDB), `pdb` (PDB ID), `corr` (path to `.corr` file), and `chain` (which chain).
 `chain` can be `_` to indicate use first chain.
 
@@ -110,16 +133,17 @@
 ```
 ## Citation
 
 Please cite [Predicting Chemical Shifts with Graph Neural Networks](https://pubs.rsc.org/en/content/articlehtml/2021/sc/d1sc01895g)
 
 ```bibtex
 @article{yang2021predicting,
-  title={Predicting Chemical Shifts with Graph Neural Networks},
+  title={Predicting chemical shifts with graph neural networks},
   author={Yang, Ziyue and Chakraborty, Maghesree and White, Andrew D},
-  journal={Chemical Science},
+  journal={Chemical science},
+  volume={12},
+  number={32},
+  pages={10802--10809},
   year={2021},
   publisher={Royal Society of Chemistry}
 }
 ```
-
-
```

### Comparing `nmrgnn-data-0.7/nmrdata/data/embeddings.pb` & `nmrgnn-data-1.1.0/nmrdata/data/embeddings.pb`

 * *Files 7% similar despite different names*

```diff
@@ -1,507 +1,518 @@
 00000000: 8003 7d71 0028 5804 0000 0061 746f 6d71  ..}q.(X....atomq
 00000010: 017d 7102 2858 0100 0000 5871 034b 0058  .}q.(X....Xq.K.X
 00000020: 0100 0000 5a71 044b 0158 0100 0000 4e71  ....Zq.K.X....Nq
 00000030: 054b 0258 0100 0000 4371 064b 0358 0100  .K.X....Cq.K.X..
 00000040: 0000 4871 074b 0458 0100 0000 4f71 084b  ..Hq.K.X....Oq.K
 00000050: 0558 0100 0000 5371 094b 0658 0100 0000  .X....Sq.K.X....
 00000060: 5071 0a4b 0758 0100 0000 4971 0b4b 0858  Pq.K.X....Iq.K.X
-00000070: 0200 0000 436c 710c 4b09 7558 0400 0000  ....Clq.K.uX....
-00000080: 626f 6e64 710d 7d71 0e28 5804 0000 006e  bondq.}q.(X....n
-00000090: 6f6e 6571 0f4b 0058 0600 0000 7369 6e67  oneq.K.X....sing
-000000a0: 6c65 7110 4b01 5806 0000 0064 6f75 626c  leq.K.X....doubl
-000000b0: 6571 114b 0258 0600 0000 7472 6970 6c65  eq.K.X....triple
-000000c0: 7112 4b03 5808 0000 0061 726f 6d61 7469  q.K.X....aromati
-000000d0: 6371 134b 0475 5803 0000 0065 7870 7114  cq.K.uX....expq.
-000000e0: 7d71 1558 0000 0000 7116 4b00 7358 0500  }q.X....q.K.sX..
-000000f0: 0000 6e6c 6973 7471 177d 7118 2868 0f4b  ..nlistq.}q.(h.K
-00000100: 0058 0900 0000 6e6f 6e62 6f6e 6465 6471  .X....nonbondedq
-00000110: 194b 014b 014b 024b 024b 034b 034b 044b  .K.K.K.K.K.K.K.K
-00000120: 044b 054b 054b 064b 064b 0775 5805 0000  .K.K.K.K.K.uX...
-00000130: 0063 6c61 7373 711a 7d71 1b28 5803 0000  .classq.}q.(X...
-00000140: 0041 4c41 711c 4b00 5803 0000 0041 5247  .ALAq.K.X....ARG
-00000150: 711d 4b01 5803 0000 0041 534e 711e 4b02  q.K.X....ASNq.K.
-00000160: 5803 0000 0041 5350 711f 4b03 5803 0000  X....ASPq.K.X...
-00000170: 0043 5953 7120 4b04 5803 0000 0047 4c55  .CYSq K.X....GLU
-00000180: 7121 4b05 5803 0000 0047 4c4e 7122 4b06  q!K.X....GLNq"K.
-00000190: 5803 0000 0047 4c59 7123 4b07 5803 0000  X....GLYq#K.X...
-000001a0: 0048 4953 7124 4b08 5803 0000 0049 4c45  .HISq$K.X....ILE
-000001b0: 7125 4b09 5803 0000 004c 4555 7126 4b0a  q%K.X....LEUq&K.
-000001c0: 5803 0000 004c 5953 7127 4b0b 5803 0000  X....LYSq'K.X...
-000001d0: 004d 4554 7128 4b0c 5803 0000 0050 4845  .METq(K.X....PHE
-000001e0: 7129 4b0d 5803 0000 0050 524f 712a 4b0e  q)K.X....PROq*K.
-000001f0: 5803 0000 0053 4552 712b 4b0f 5803 0000  X....SERq+K.X...
-00000200: 0054 4852 712c 4b10 5803 0000 0054 5250  .THRq,K.X....TRP
-00000210: 712d 4b11 5803 0000 0054 5952 712e 4b12  q-K.X....TYRq.K.
-00000220: 5803 0000 0056 414c 712f 4b13 5802 0000  X....VALq/K.X...
-00000230: 004d 4271 304b 1458 0300 0000 4446 5471  .MBq0K.X....DFTq
-00000240: 314b 1575 5804 0000 006e 616d 6571 327d  1K.uX....nameq2}
-00000250: 7133 2868 034b 0058 0400 0000 4d42 2d4e  q3(h.K.X....MB-N
-00000260: 7134 4b01 5804 0000 004d 422d 4371 354b  q4K.X....MB-Cq5K
-00000270: 0258 0400 0000 4d42 2d48 7136 4b03 5804  .X....MB-Hq6K.X.
-00000280: 0000 004d 422d 4f71 374b 0458 0400 0000  ...MB-Oq7K.X....
-00000290: 4d42 2d53 7138 4b05 5804 0000 004d 422d  MB-Sq8K.X....MB-
-000002a0: 5071 394b 0658 0400 0000 4d42 2d49 713a  Pq9K.X....MB-Iq:
-000002b0: 4b07 5805 0000 004d 422d 436c 713b 4b08  K.X....MB-Clq;K.
-000002c0: 5805 0000 0050 524f 2d4e 713c 4b09 5806  X....PRO-Nq<K.X.
-000002d0: 0000 0050 524f 2d43 4171 3d4b 0a58 0500  ...PRO-CAq=K.X..
-000002e0: 0000 5052 4f2d 4371 3e4b 0b58 0500 0000  ..PRO-Cq>K.X....
-000002f0: 5052 4f2d 4f71 3f4b 0c58 0600 0000 5052  PRO-Oq?K.X....PR
-00000300: 4f2d 4342 7140 4b0d 5806 0000 0050 524f  O-CBq@K.X....PRO
-00000310: 2d43 4771 414b 0e58 0600 0000 5052 4f2d  -CGqAK.X....PRO-
-00000320: 4344 7142 4b0f 5805 0000 0050 524f 2d48  CDqBK.X....PRO-H
-00000330: 7143 4b10 5806 0000 0050 524f 2d48 3371  qCK.X....PRO-H3q
-00000340: 444b 1158 0600 0000 5052 4f2d 4841 7145  DK.X....PRO-HAqE
-00000350: 4b12 5807 0000 0050 524f 2d48 4232 7146  K.X....PRO-HB2qF
-00000360: 4b13 5807 0000 0050 524f 2d48 4233 7147  K.X....PRO-HB3qG
-00000370: 4b14 5807 0000 0050 524f 2d48 4732 7148  K.X....PRO-HG2qH
-00000380: 4b15 5807 0000 0050 524f 2d48 4733 7149  K.X....PRO-HG3qI
-00000390: 4b16 5807 0000 0050 524f 2d48 4432 714a  K.X....PRO-HD2qJ
-000003a0: 4b17 5807 0000 0050 524f 2d48 4433 714b  K.X....PRO-HD3qK
-000003b0: 4b18 5805 0000 0049 4c45 2d4e 714c 4b19  K.X....ILE-NqLK.
-000003c0: 5806 0000 0049 4c45 2d43 4171 4d4b 1a58  X....ILE-CAqMK.X
-000003d0: 0500 0000 494c 452d 4371 4e4b 1b58 0500  ....ILE-CqNK.X..
-000003e0: 0000 494c 452d 4f71 4f4b 1c58 0600 0000  ..ILE-OqOK.X....
-000003f0: 494c 452d 4342 7150 4b1d 5807 0000 0049  ILE-CBqPK.X....I
-00000400: 4c45 2d43 4731 7151 4b1e 5807 0000 0049  LE-CG1qQK.X....I
-00000410: 4c45 2d43 4732 7152 4b1f 5807 0000 0049  LE-CG2qRK.X....I
-00000420: 4c45 2d43 4431 7153 4b20 5805 0000 0049  LE-CD1qSK X....I
-00000430: 4c45 2d48 7154 4b21 5806 0000 0049 4c45  LE-HqTK!X....ILE
-00000440: 2d48 4171 554b 2258 0600 0000 494c 452d  -HAqUK"X....ILE-
-00000450: 4842 7156 4b23 5808 0000 0049 4c45 2d48  HBqVK#X....ILE-H
-00000460: 4731 3271 574b 2458 0800 0000 494c 452d  G12qWK$X....ILE-
-00000470: 4847 3133 7158 4b25 5808 0000 0049 4c45  HG13qXK%X....ILE
-00000480: 2d48 4732 3171 594b 2658 0800 0000 494c  -HG21qYK&X....IL
-00000490: 452d 4847 3232 715a 4b27 5808 0000 0049  E-HG22qZK'X....I
-000004a0: 4c45 2d48 4732 3371 5b4b 2858 0800 0000  LE-HG23q[K(X....
-000004b0: 494c 452d 4844 3131 715c 4b29 5808 0000  ILE-HD11q\K)X...
-000004c0: 0049 4c45 2d48 4431 3271 5d4b 2a58 0800  .ILE-HD12q]K*X..
-000004d0: 0000 494c 452d 4844 3133 715e 4b2b 5805  ..ILE-HD13q^K+X.
-000004e0: 0000 0056 414c 2d4e 715f 4b2c 5806 0000  ...VAL-Nq_K,X...
-000004f0: 0056 414c 2d43 4171 604b 2d58 0500 0000  .VAL-CAq`K-X....
-00000500: 5641 4c2d 4371 614b 2e58 0500 0000 5641  VAL-CqaK.X....VA
-00000510: 4c2d 4f71 624b 2f58 0600 0000 5641 4c2d  L-OqbK/X....VAL-
-00000520: 4342 7163 4b30 5807 0000 0056 414c 2d43  CBqcK0X....VAL-C
-00000530: 4731 7164 4b31 5807 0000 0056 414c 2d43  G1qdK1X....VAL-C
-00000540: 4732 7165 4b32 5805 0000 0056 414c 2d48  G2qeK2X....VAL-H
-00000550: 7166 4b33 5806 0000 0056 414c 2d48 4171  qfK3X....VAL-HAq
-00000560: 674b 3458 0600 0000 5641 4c2d 4842 7168  gK4X....VAL-HBqh
-00000570: 4b35 5808 0000 0056 414c 2d48 4731 3171  K5X....VAL-HG11q
-00000580: 694b 3658 0800 0000 5641 4c2d 4847 3132  iK6X....VAL-HG12
-00000590: 716a 4b37 5808 0000 0056 414c 2d48 4731  qjK7X....VAL-HG1
-000005a0: 3371 6b4b 3858 0800 0000 5641 4c2d 4847  3qkK8X....VAL-HG
-000005b0: 3231 716c 4b39 5808 0000 0056 414c 2d48  21qlK9X....VAL-H
-000005c0: 4732 3271 6d4b 3a58 0800 0000 5641 4c2d  G22qmK:X....VAL-
-000005d0: 4847 3233 716e 4b3b 5805 0000 0041 5247  HG23qnK;X....ARG
-000005e0: 2d4e 716f 4b3c 5806 0000 0041 5247 2d43  -NqoK<X....ARG-C
-000005f0: 4171 704b 3d58 0500 0000 4152 472d 4371  AqpK=X....ARG-Cq
-00000600: 714b 3e58 0500 0000 4152 472d 4f71 724b  qK>X....ARG-OqrK
-00000610: 3f58 0600 0000 4152 472d 4342 7173 4b40  ?X....ARG-CBqsK@
-00000620: 5806 0000 0041 5247 2d43 4771 744b 4158  X....ARG-CGqtKAX
-00000630: 0600 0000 4152 472d 4344 7175 4b42 5806  ....ARG-CDquKBX.
-00000640: 0000 0041 5247 2d4e 4571 764b 4358 0600  ...ARG-NEqvKCX..
-00000650: 0000 4152 472d 435a 7177 4b44 5807 0000  ..ARG-CZqwKDX...
-00000660: 0041 5247 2d4e 4831 7178 4b45 5807 0000  .ARG-NH1qxKEX...
-00000670: 0041 5247 2d4e 4832 7179 4b46 5805 0000  .ARG-NH2qyKFX...
-00000680: 0041 5247 2d48 717a 4b47 5806 0000 0041  .ARG-HqzKGX....A
-00000690: 5247 2d48 4171 7b4b 4858 0700 0000 4152  RG-HAq{KHX....AR
-000006a0: 472d 4842 3271 7c4b 4958 0700 0000 4152  G-HB2q|KIX....AR
-000006b0: 472d 4842 3371 7d4b 4a58 0700 0000 4152  G-HB3q}KJX....AR
-000006c0: 472d 4847 3271 7e4b 4b58 0700 0000 4152  G-HG2q~KKX....AR
-000006d0: 472d 4847 3371 7f4b 4c58 0700 0000 4152  G-HG3q.KLX....AR
-000006e0: 472d 4844 3271 804b 4d58 0700 0000 4152  G-HD2q.KMX....AR
-000006f0: 472d 4844 3371 814b 4e58 0600 0000 4152  G-HD3q.KNX....AR
-00000700: 472d 4845 7182 4b4f 5808 0000 0041 5247  G-HEq.KOX....ARG
-00000710: 2d48 4831 3171 834b 5058 0800 0000 4152  -HH11q.KPX....AR
-00000720: 472d 4848 3132 7184 4b51 5808 0000 0041  G-HH12q.KQX....A
-00000730: 5247 2d48 4832 3171 854b 5258 0800 0000  RG-HH21q.KRX....
-00000740: 4152 472d 4848 3232 7186 4b53 5805 0000  ARG-HH22q.KSX...
-00000750: 004c 5953 2d4e 7187 4b54 5806 0000 004c  .LYS-Nq.KTX....L
-00000760: 5953 2d43 4171 884b 5558 0500 0000 4c59  YS-CAq.KUX....LY
-00000770: 532d 4371 894b 5658 0500 0000 4c59 532d  S-Cq.KVX....LYS-
-00000780: 4f71 8a4b 5758 0600 0000 4c59 532d 4342  Oq.KWX....LYS-CB
-00000790: 718b 4b58 5806 0000 004c 5953 2d43 4771  q.KXX....LYS-CGq
-000007a0: 8c4b 5958 0600 0000 4c59 532d 4344 718d  .KYX....LYS-CDq.
-000007b0: 4b5a 5806 0000 004c 5953 2d43 4571 8e4b  KZX....LYS-CEq.K
-000007c0: 5b58 0600 0000 4c59 532d 4e5a 718f 4b5c  [X....LYS-NZq.K\
-000007d0: 5805 0000 004c 5953 2d48 7190 4b5d 5806  X....LYS-Hq.K]X.
-000007e0: 0000 004c 5953 2d48 4171 914b 5e58 0700  ...LYS-HAq.K^X..
-000007f0: 0000 4c59 532d 4842 3271 924b 5f58 0700  ..LYS-HB2q.K_X..
-00000800: 0000 4c59 532d 4842 3371 934b 6058 0700  ..LYS-HB3q.K`X..
-00000810: 0000 4c59 532d 4847 3271 944b 6158 0700  ..LYS-HG2q.KaX..
-00000820: 0000 4c59 532d 4847 3371 954b 6258 0700  ..LYS-HG3q.KbX..
-00000830: 0000 4c59 532d 4844 3271 964b 6358 0700  ..LYS-HD2q.KcX..
-00000840: 0000 4c59 532d 4844 3371 974b 6458 0700  ..LYS-HD3q.KdX..
-00000850: 0000 4c59 532d 4845 3271 984b 6558 0700  ..LYS-HE2q.KeX..
-00000860: 0000 4c59 532d 4845 3371 994b 6658 0700  ..LYS-HE3q.KfX..
-00000870: 0000 4c59 532d 485a 3171 9a4b 6758 0700  ..LYS-HZ1q.KgX..
-00000880: 0000 4c59 532d 485a 3271 9b4b 6858 0700  ..LYS-HZ2q.KhX..
-00000890: 0000 4c59 532d 485a 3371 9c4b 6958 0500  ..LYS-HZ3q.KiX..
-000008a0: 0000 474c 552d 4e71 9d4b 6a58 0600 0000  ..GLU-Nq.KjX....
-000008b0: 474c 552d 4341 719e 4b6b 5805 0000 0047  GLU-CAq.KkX....G
-000008c0: 4c55 2d43 719f 4b6c 5805 0000 0047 4c55  LU-Cq.KlX....GLU
-000008d0: 2d4f 71a0 4b6d 5806 0000 0047 4c55 2d43  -Oq.KmX....GLU-C
-000008e0: 4271 a14b 6e58 0600 0000 474c 552d 4347  Bq.KnX....GLU-CG
-000008f0: 71a2 4b6f 5806 0000 0047 4c55 2d43 4471  q.KoX....GLU-CDq
-00000900: a34b 7058 0700 0000 474c 552d 4f45 3171  .KpX....GLU-OE1q
-00000910: a44b 7158 0700 0000 474c 552d 4f45 3271  .KqX....GLU-OE2q
-00000920: a54b 7258 0500 0000 474c 552d 4871 a64b  .KrX....GLU-Hq.K
-00000930: 7358 0600 0000 474c 552d 4841 71a7 4b74  sX....GLU-HAq.Kt
-00000940: 5807 0000 0047 4c55 2d48 4232 71a8 4b75  X....GLU-HB2q.Ku
-00000950: 5807 0000 0047 4c55 2d48 4233 71a9 4b76  X....GLU-HB3q.Kv
-00000960: 5807 0000 0047 4c55 2d48 4732 71aa 4b77  X....GLU-HG2q.Kw
-00000970: 5807 0000 0047 4c55 2d48 4733 71ab 4b78  X....GLU-HG3q.Kx
-00000980: 5805 0000 004c 4555 2d4e 71ac 4b79 5806  X....LEU-Nq.KyX.
-00000990: 0000 004c 4555 2d43 4171 ad4b 7a58 0500  ...LEU-CAq.KzX..
-000009a0: 0000 4c45 552d 4371 ae4b 7b58 0500 0000  ..LEU-Cq.K{X....
-000009b0: 4c45 552d 4f71 af4b 7c58 0600 0000 4c45  LEU-Oq.K|X....LE
-000009c0: 552d 4342 71b0 4b7d 5806 0000 004c 4555  U-CBq.K}X....LEU
-000009d0: 2d43 4771 b14b 7e58 0700 0000 4c45 552d  -CGq.K~X....LEU-
-000009e0: 4344 3171 b24b 7f58 0700 0000 4c45 552d  CD1q.K.X....LEU-
-000009f0: 4344 3271 b34b 8058 0500 0000 4c45 552d  CD2q.K.X....LEU-
-00000a00: 4871 b44b 8158 0600 0000 4c45 552d 4841  Hq.K.X....LEU-HA
-00000a10: 71b5 4b82 5807 0000 004c 4555 2d48 4232  q.K.X....LEU-HB2
-00000a20: 71b6 4b83 5807 0000 004c 4555 2d48 4233  q.K.X....LEU-HB3
-00000a30: 71b7 4b84 5806 0000 004c 4555 2d48 4771  q.K.X....LEU-HGq
-00000a40: b84b 8558 0800 0000 4c45 552d 4844 3131  .K.X....LEU-HD11
-00000a50: 71b9 4b86 5808 0000 004c 4555 2d48 4431  q.K.X....LEU-HD1
-00000a60: 3271 ba4b 8758 0800 0000 4c45 552d 4844  2q.K.X....LEU-HD
-00000a70: 3133 71bb 4b88 5808 0000 004c 4555 2d48  13q.K.X....LEU-H
-00000a80: 4432 3171 bc4b 8958 0800 0000 4c45 552d  D21q.K.X....LEU-
-00000a90: 4844 3232 71bd 4b8a 5808 0000 004c 4555  HD22q.K.X....LEU
-00000aa0: 2d48 4432 3371 be4b 8b58 0500 0000 5459  -HD23q.K.X....TY
-00000ab0: 522d 4e71 bf4b 8c58 0600 0000 5459 522d  R-Nq.K.X....TYR-
-00000ac0: 4341 71c0 4b8d 5805 0000 0054 5952 2d43  CAq.K.X....TYR-C
-00000ad0: 71c1 4b8e 5805 0000 0054 5952 2d4f 71c2  q.K.X....TYR-Oq.
-00000ae0: 4b8f 5806 0000 0054 5952 2d43 4271 c34b  K.X....TYR-CBq.K
-00000af0: 9058 0600 0000 5459 522d 4347 71c4 4b91  .X....TYR-CGq.K.
-00000b00: 5807 0000 0054 5952 2d43 4431 71c5 4b92  X....TYR-CD1q.K.
-00000b10: 5807 0000 0054 5952 2d43 4432 71c6 4b93  X....TYR-CD2q.K.
-00000b20: 5807 0000 0054 5952 2d43 4531 71c7 4b94  X....TYR-CE1q.K.
-00000b30: 5807 0000 0054 5952 2d43 4532 71c8 4b95  X....TYR-CE2q.K.
-00000b40: 5806 0000 0054 5952 2d43 5a71 c94b 9658  X....TYR-CZq.K.X
-00000b50: 0600 0000 5459 522d 4f48 71ca 4b97 5805  ....TYR-OHq.K.X.
-00000b60: 0000 0054 5952 2d48 71cb 4b98 5806 0000  ...TYR-Hq.K.X...
-00000b70: 0054 5952 2d48 4171 cc4b 9958 0700 0000  .TYR-HAq.K.X....
-00000b80: 5459 522d 4842 3271 cd4b 9a58 0700 0000  TYR-HB2q.K.X....
-00000b90: 5459 522d 4842 3371 ce4b 9b58 0700 0000  TYR-HB3q.K.X....
-00000ba0: 5459 522d 4844 3171 cf4b 9c58 0700 0000  TYR-HD1q.K.X....
-00000bb0: 5459 522d 4844 3271 d04b 9d58 0700 0000  TYR-HD2q.K.X....
-00000bc0: 5459 522d 4845 3171 d14b 9e58 0700 0000  TYR-HE1q.K.X....
-00000bd0: 5459 522d 4845 3271 d24b 9f58 0600 0000  TYR-HE2q.K.X....
-00000be0: 5459 522d 4848 71d3 4ba0 5805 0000 0043  TYR-HHq.K.X....C
-00000bf0: 5953 2d4e 71d4 4ba1 5806 0000 0043 5953  YS-Nq.K.X....CYS
-00000c00: 2d43 4171 d54b a258 0500 0000 4359 532d  -CAq.K.X....CYS-
-00000c10: 4371 d64b a358 0500 0000 4359 532d 4f71  Cq.K.X....CYS-Oq
-00000c20: d74b a458 0600 0000 4359 532d 4342 71d8  .K.X....CYS-CBq.
-00000c30: 4ba5 5806 0000 0043 5953 2d53 4771 d94b  K.X....CYS-SGq.K
-00000c40: a658 0500 0000 4359 532d 4871 da4b a758  .X....CYS-Hq.K.X
-00000c50: 0600 0000 4359 532d 4841 71db 4ba8 5807  ....CYS-HAq.K.X.
-00000c60: 0000 0043 5953 2d48 4232 71dc 4ba9 5807  ...CYS-HB2q.K.X.
-00000c70: 0000 0043 5953 2d48 4233 71dd 4baa 5806  ...CYS-HB3q.K.X.
-00000c80: 0000 0043 5953 2d48 4771 de4b ab58 0500  ...CYS-HGq.K.X..
-00000c90: 0000 474c 592d 4e71 df4b ac58 0600 0000  ..GLY-Nq.K.X....
-00000ca0: 474c 592d 4341 71e0 4bad 5805 0000 0047  GLY-CAq.K.X....G
-00000cb0: 4c59 2d43 71e1 4bae 5805 0000 0047 4c59  LY-Cq.K.X....GLY
-00000cc0: 2d4f 71e2 4baf 5805 0000 0047 4c59 2d48  -Oq.K.X....GLY-H
-00000cd0: 71e3 4bb0 5807 0000 0047 4c59 2d48 4132  q.K.X....GLY-HA2
-00000ce0: 71e4 4bb1 5807 0000 0047 4c59 2d48 4133  q.K.X....GLY-HA3
-00000cf0: 71e5 4bb2 5805 0000 0050 4845 2d4e 71e6  q.K.X....PHE-Nq.
-00000d00: 4bb3 5806 0000 0050 4845 2d43 4171 e74b  K.X....PHE-CAq.K
-00000d10: b458 0500 0000 5048 452d 4371 e84b b558  .X....PHE-Cq.K.X
-00000d20: 0500 0000 5048 452d 4f71 e94b b658 0600  ....PHE-Oq.K.X..
-00000d30: 0000 5048 452d 4342 71ea 4bb7 5806 0000  ..PHE-CBq.K.X...
-00000d40: 0050 4845 2d43 4771 eb4b b858 0700 0000  .PHE-CGq.K.X....
-00000d50: 5048 452d 4344 3171 ec4b b958 0700 0000  PHE-CD1q.K.X....
-00000d60: 5048 452d 4344 3271 ed4b ba58 0700 0000  PHE-CD2q.K.X....
-00000d70: 5048 452d 4345 3171 ee4b bb58 0700 0000  PHE-CE1q.K.X....
-00000d80: 5048 452d 4345 3271 ef4b bc58 0600 0000  PHE-CE2q.K.X....
-00000d90: 5048 452d 435a 71f0 4bbd 5805 0000 0050  PHE-CZq.K.X....P
-00000da0: 4845 2d48 71f1 4bbe 5806 0000 0050 4845  HE-Hq.K.X....PHE
-00000db0: 2d48 4171 f24b bf58 0700 0000 5048 452d  -HAq.K.X....PHE-
-00000dc0: 4842 3271 f34b c058 0700 0000 5048 452d  HB2q.K.X....PHE-
-00000dd0: 4842 3371 f44b c158 0700 0000 5048 452d  HB3q.K.X....PHE-
-00000de0: 4844 3171 f54b c258 0700 0000 5048 452d  HD1q.K.X....PHE-
-00000df0: 4844 3271 f64b c358 0700 0000 5048 452d  HD2q.K.X....PHE-
-00000e00: 4845 3171 f74b c458 0700 0000 5048 452d  HE1q.K.X....PHE-
-00000e10: 4845 3271 f84b c558 0600 0000 5048 452d  HE2q.K.X....PHE-
-00000e20: 485a 71f9 4bc6 5805 0000 0041 4c41 2d4e  HZq.K.X....ALA-N
-00000e30: 71fa 4bc7 5806 0000 0041 4c41 2d43 4171  q.K.X....ALA-CAq
-00000e40: fb4b c858 0500 0000 414c 412d 4371 fc4b  .K.X....ALA-Cq.K
-00000e50: c958 0500 0000 414c 412d 4f71 fd4b ca58  .X....ALA-Oq.K.X
-00000e60: 0600 0000 414c 412d 4342 71fe 4bcb 5805  ....ALA-CBq.K.X.
-00000e70: 0000 0041 4c41 2d48 71ff 4bcc 5806 0000  ...ALA-Hq.K.X...
-00000e80: 0041 4c41 2d48 4172 0001 0000 4bcd 5807  .ALA-HAr....K.X.
-00000e90: 0000 0041 4c41 2d48 4231 7201 0100 004b  ...ALA-HB1r....K
-00000ea0: ce58 0700 0000 414c 412d 4842 3272 0201  .X....ALA-HB2r..
-00000eb0: 0000 4bcf 5807 0000 0041 4c41 2d48 4233  ..K.X....ALA-HB3
-00000ec0: 7203 0100 004b d058 0500 0000 474c 4e2d  r....K.X....GLN-
-00000ed0: 4e72 0401 0000 4bd1 5806 0000 0047 4c4e  Nr....K.X....GLN
-00000ee0: 2d43 4172 0501 0000 4bd2 5805 0000 0047  -CAr....K.X....G
-00000ef0: 4c4e 2d43 7206 0100 004b d358 0500 0000  LN-Cr....K.X....
-00000f00: 474c 4e2d 4f72 0701 0000 4bd4 5806 0000  GLN-Or....K.X...
-00000f10: 0047 4c4e 2d43 4272 0801 0000 4bd5 5806  .GLN-CBr....K.X.
-00000f20: 0000 0047 4c4e 2d43 4772 0901 0000 4bd6  ...GLN-CGr....K.
-00000f30: 5806 0000 0047 4c4e 2d43 4472 0a01 0000  X....GLN-CDr....
-00000f40: 4bd7 5807 0000 0047 4c4e 2d4f 4531 720b  K.X....GLN-OE1r.
-00000f50: 0100 004b d858 0700 0000 474c 4e2d 4e45  ...K.X....GLN-NE
-00000f60: 3272 0c01 0000 4bd9 5805 0000 0047 4c4e  2r....K.X....GLN
-00000f70: 2d48 720d 0100 004b da58 0600 0000 474c  -Hr....K.X....GL
-00000f80: 4e2d 4841 720e 0100 004b db58 0700 0000  N-HAr....K.X....
-00000f90: 474c 4e2d 4842 3272 0f01 0000 4bdc 5807  GLN-HB2r....K.X.
-00000fa0: 0000 0047 4c4e 2d48 4233 7210 0100 004b  ...GLN-HB3r....K
-00000fb0: dd58 0700 0000 474c 4e2d 4847 3272 1101  .X....GLN-HG2r..
-00000fc0: 0000 4bde 5807 0000 0047 4c4e 2d48 4733  ..K.X....GLN-HG3
-00000fd0: 7212 0100 004b df58 0800 0000 474c 4e2d  r....K.X....GLN-
-00000fe0: 4845 3231 7213 0100 004b e058 0800 0000  HE21r....K.X....
-00000ff0: 474c 4e2d 4845 3232 7214 0100 004b e158  GLN-HE22r....K.X
-00001000: 0500 0000 4153 502d 4e72 1501 0000 4be2  ....ASP-Nr....K.
-00001010: 5806 0000 0041 5350 2d43 4172 1601 0000  X....ASP-CAr....
-00001020: 4be3 5805 0000 0041 5350 2d43 7217 0100  K.X....ASP-Cr...
-00001030: 004b e458 0500 0000 4153 502d 4f72 1801  .K.X....ASP-Or..
-00001040: 0000 4be5 5806 0000 0041 5350 2d43 4272  ..K.X....ASP-CBr
-00001050: 1901 0000 4be6 5806 0000 0041 5350 2d43  ....K.X....ASP-C
-00001060: 4772 1a01 0000 4be7 5807 0000 0041 5350  Gr....K.X....ASP
-00001070: 2d4f 4431 721b 0100 004b e858 0700 0000  -OD1r....K.X....
-00001080: 4153 502d 4f44 3272 1c01 0000 4be9 5805  ASP-OD2r....K.X.
-00001090: 0000 0041 5350 2d48 721d 0100 004b ea58  ...ASP-Hr....K.X
-000010a0: 0600 0000 4153 502d 4841 721e 0100 004b  ....ASP-HAr....K
-000010b0: eb58 0700 0000 4153 502d 4842 3272 1f01  .X....ASP-HB2r..
-000010c0: 0000 4bec 5807 0000 0041 5350 2d48 4233  ..K.X....ASP-HB3
-000010d0: 7220 0100 004b ed58 0500 0000 4849 532d  r ...K.X....HIS-
-000010e0: 4e72 2101 0000 4bee 5806 0000 0048 4953  Nr!...K.X....HIS
-000010f0: 2d43 4172 2201 0000 4bef 5805 0000 0048  -CAr"...K.X....H
-00001100: 4953 2d43 7223 0100 004b f058 0500 0000  IS-Cr#...K.X....
-00001110: 4849 532d 4f72 2401 0000 4bf1 5806 0000  HIS-Or$...K.X...
-00001120: 0048 4953 2d43 4272 2501 0000 4bf2 5806  .HIS-CBr%...K.X.
-00001130: 0000 0048 4953 2d43 4772 2601 0000 4bf3  ...HIS-CGr&...K.
-00001140: 5807 0000 0048 4953 2d4e 4431 7227 0100  X....HIS-ND1r'..
-00001150: 004b f458 0700 0000 4849 532d 4344 3272  .K.X....HIS-CD2r
-00001160: 2801 0000 4bf5 5807 0000 0048 4953 2d43  (...K.X....HIS-C
-00001170: 4531 7229 0100 004b f658 0700 0000 4849  E1r)...K.X....HI
-00001180: 532d 4e45 3272 2a01 0000 4bf7 5805 0000  S-NE2r*...K.X...
-00001190: 0048 4953 2d48 722b 0100 004b f858 0600  .HIS-Hr+...K.X..
-000011a0: 0000 4849 532d 4841 722c 0100 004b f958  ..HIS-HAr,...K.X
-000011b0: 0700 0000 4849 532d 4842 3272 2d01 0000  ....HIS-HB2r-...
-000011c0: 4bfa 5807 0000 0048 4953 2d48 4233 722e  K.X....HIS-HB3r.
-000011d0: 0100 004b fb58 0700 0000 4849 532d 4844  ...K.X....HIS-HD
-000011e0: 3172 2f01 0000 4bfc 5807 0000 0048 4953  1r/...K.X....HIS
-000011f0: 2d48 4432 7230 0100 004b fd58 0700 0000  -HD2r0...K.X....
-00001200: 4849 532d 4845 3172 3101 0000 4bfe 5807  HIS-HE1r1...K.X.
-00001210: 0000 0048 4953 2d48 4532 7232 0100 004b  ...HIS-HE2r2...K
-00001220: ff58 0500 0000 5345 522d 4e72 3301 0000  .X....SER-Nr3...
-00001230: 4d00 0158 0600 0000 5345 522d 4341 7234  M..X....SER-CAr4
-00001240: 0100 004d 0101 5805 0000 0053 4552 2d43  ...M..X....SER-C
-00001250: 7235 0100 004d 0201 5805 0000 0053 4552  r5...M..X....SER
-00001260: 2d4f 7236 0100 004d 0301 5806 0000 0053  -Or6...M..X....S
-00001270: 4552 2d43 4272 3701 0000 4d04 0158 0600  ER-CBr7...M..X..
-00001280: 0000 5345 522d 4f47 7238 0100 004d 0501  ..SER-OGr8...M..
-00001290: 5805 0000 0053 4552 2d48 7239 0100 004d  X....SER-Hr9...M
-000012a0: 0601 5806 0000 0053 4552 2d48 4172 3a01  ..X....SER-HAr:.
-000012b0: 0000 4d07 0158 0700 0000 5345 522d 4842  ..M..X....SER-HB
-000012c0: 3272 3b01 0000 4d08 0158 0700 0000 5345  2r;...M..X....SE
-000012d0: 522d 4842 3372 3c01 0000 4d09 0158 0600  R-HB3r<...M..X..
-000012e0: 0000 5345 522d 4847 723d 0100 004d 0a01  ..SER-HGr=...M..
-000012f0: 5805 0000 0054 4852 2d4e 723e 0100 004d  X....THR-Nr>...M
-00001300: 0b01 5806 0000 0054 4852 2d43 4172 3f01  ..X....THR-CAr?.
-00001310: 0000 4d0c 0158 0500 0000 5448 522d 4372  ..M..X....THR-Cr
-00001320: 4001 0000 4d0d 0158 0500 0000 5448 522d  @...M..X....THR-
-00001330: 4f72 4101 0000 4d0e 0158 0600 0000 5448  OrA...M..X....TH
-00001340: 522d 4342 7242 0100 004d 0f01 5807 0000  R-CBrB...M..X...
-00001350: 0054 4852 2d4f 4731 7243 0100 004d 1001  .THR-OG1rC...M..
-00001360: 5807 0000 0054 4852 2d43 4732 7244 0100  X....THR-CG2rD..
-00001370: 004d 1101 5805 0000 0054 4852 2d48 7245  .M..X....THR-HrE
-00001380: 0100 004d 1201 5806 0000 0054 4852 2d48  ...M..X....THR-H
-00001390: 4172 4601 0000 4d13 0158 0600 0000 5448  ArF...M..X....TH
-000013a0: 522d 4842 7247 0100 004d 1401 5807 0000  R-HBrG...M..X...
-000013b0: 0054 4852 2d48 4731 7248 0100 004d 1501  .THR-HG1rH...M..
-000013c0: 5808 0000 0054 4852 2d48 4732 3172 4901  X....THR-HG21rI.
-000013d0: 0000 4d16 0158 0800 0000 5448 522d 4847  ..M..X....THR-HG
-000013e0: 3232 724a 0100 004d 1701 5808 0000 0054  22rJ...M..X....T
-000013f0: 4852 2d48 4732 3372 4b01 0000 4d18 0158  HR-HG23rK...M..X
-00001400: 0500 0000 4153 4e2d 4e72 4c01 0000 4d19  ....ASN-NrL...M.
-00001410: 0158 0600 0000 4153 4e2d 4341 724d 0100  .X....ASN-CArM..
-00001420: 004d 1a01 5805 0000 0041 534e 2d43 724e  .M..X....ASN-CrN
-00001430: 0100 004d 1b01 5805 0000 0041 534e 2d4f  ...M..X....ASN-O
-00001440: 724f 0100 004d 1c01 5806 0000 0041 534e  rO...M..X....ASN
-00001450: 2d43 4272 5001 0000 4d1d 0158 0600 0000  -CBrP...M..X....
-00001460: 4153 4e2d 4347 7251 0100 004d 1e01 5807  ASN-CGrQ...M..X.
-00001470: 0000 0041 534e 2d4f 4431 7252 0100 004d  ...ASN-OD1rR...M
-00001480: 1f01 5807 0000 0041 534e 2d4e 4432 7253  ..X....ASN-ND2rS
-00001490: 0100 004d 2001 5805 0000 0041 534e 2d48  ...M .X....ASN-H
-000014a0: 7254 0100 004d 2101 5806 0000 0041 534e  rT...M!.X....ASN
-000014b0: 2d48 4172 5501 0000 4d22 0158 0700 0000  -HArU...M".X....
-000014c0: 4153 4e2d 4842 3272 5601 0000 4d23 0158  ASN-HB2rV...M#.X
-000014d0: 0700 0000 4153 4e2d 4842 3372 5701 0000  ....ASN-HB3rW...
-000014e0: 4d24 0158 0800 0000 4153 4e2d 4844 3231  M$.X....ASN-HD21
-000014f0: 7258 0100 004d 2501 5808 0000 0041 534e  rX...M%.X....ASN
-00001500: 2d48 4432 3272 5901 0000 4d26 0158 0700  -HD22rY...M&.X..
-00001510: 0000 414c 412d 4f58 5472 5a01 0000 4d27  ..ALA-OXTrZ...M'
-00001520: 0158 0600 0000 414c 412d 4832 725b 0100  .X....ALA-H2r[..
-00001530: 004d 2801 5806 0000 0041 4c41 2d48 3372  .M(.X....ALA-H3r
-00001540: 5c01 0000 4d29 0158 0700 0000 474c 552d  \...M).X....GLU-
-00001550: 4845 3272 5d01 0000 4d2a 0158 0700 0000  HE2r]...M*.X....
-00001560: 4153 502d 4844 3272 5e01 0000 4d2b 0158  ASP-HD2r^...M+.X
-00001570: 0500 0000 4d45 542d 4e72 5f01 0000 4d2c  ....MET-Nr_...M,
-00001580: 0158 0600 0000 4d45 542d 4341 7260 0100  .X....MET-CAr`..
-00001590: 004d 2d01 5805 0000 004d 4554 2d43 7261  .M-.X....MET-Cra
-000015a0: 0100 004d 2e01 5805 0000 004d 4554 2d4f  ...M..X....MET-O
-000015b0: 7262 0100 004d 2f01 5806 0000 004d 4554  rb...M/.X....MET
-000015c0: 2d43 4272 6301 0000 4d30 0158 0600 0000  -CBrc...M0.X....
-000015d0: 4d45 542d 4347 7264 0100 004d 3101 5806  MET-CGrd...M1.X.
-000015e0: 0000 004d 4554 2d53 4472 6501 0000 4d32  ...MET-SDre...M2
-000015f0: 0158 0600 0000 4d45 542d 4345 7266 0100  .X....MET-CErf..
-00001600: 004d 3301 5805 0000 004d 4554 2d48 7267  .M3.X....MET-Hrg
-00001610: 0100 004d 3401 5806 0000 004d 4554 2d48  ...M4.X....MET-H
-00001620: 4172 6801 0000 4d35 0158 0700 0000 4d45  Arh...M5.X....ME
-00001630: 542d 4842 3272 6901 0000 4d36 0158 0700  T-HB2ri...M6.X..
-00001640: 0000 4d45 542d 4842 3372 6a01 0000 4d37  ..MET-HB3rj...M7
-00001650: 0158 0700 0000 4d45 542d 4847 3272 6b01  .X....MET-HG2rk.
-00001660: 0000 4d38 0158 0700 0000 4d45 542d 4847  ..M8.X....MET-HG
-00001670: 3372 6c01 0000 4d39 0158 0700 0000 4d45  3rl...M9.X....ME
-00001680: 542d 4845 3172 6d01 0000 4d3a 0158 0700  T-HE1rm...M:.X..
-00001690: 0000 4d45 542d 4845 3272 6e01 0000 4d3b  ..MET-HE2rn...M;
-000016a0: 0158 0700 0000 4d45 542d 4845 3372 6f01  .X....MET-HE3ro.
-000016b0: 0000 4d3c 0158 0500 0000 5452 502d 4e72  ..M<.X....TRP-Nr
-000016c0: 7001 0000 4d3d 0158 0600 0000 5452 502d  p...M=.X....TRP-
-000016d0: 4341 7271 0100 004d 3e01 5805 0000 0054  CArq...M>.X....T
-000016e0: 5250 2d43 7272 0100 004d 3f01 5805 0000  RP-Crr...M?.X...
-000016f0: 0054 5250 2d4f 7273 0100 004d 4001 5806  .TRP-Ors...M@.X.
-00001700: 0000 0054 5250 2d43 4272 7401 0000 4d41  ...TRP-CBrt...MA
-00001710: 0158 0600 0000 5452 502d 4347 7275 0100  .X....TRP-CGru..
-00001720: 004d 4201 5807 0000 0054 5250 2d43 4431  .MB.X....TRP-CD1
-00001730: 7276 0100 004d 4301 5807 0000 0054 5250  rv...MC.X....TRP
-00001740: 2d43 4432 7277 0100 004d 4401 5807 0000  -CD2rw...MD.X...
-00001750: 0054 5250 2d4e 4531 7278 0100 004d 4501  .TRP-NE1rx...ME.
-00001760: 5807 0000 0054 5250 2d43 4532 7279 0100  X....TRP-CE2ry..
-00001770: 004d 4601 5807 0000 0054 5250 2d43 4533  .MF.X....TRP-CE3
-00001780: 727a 0100 004d 4701 5807 0000 0054 5250  rz...MG.X....TRP
-00001790: 2d43 5a32 727b 0100 004d 4801 5807 0000  -CZ2r{...MH.X...
-000017a0: 0054 5250 2d43 5a33 727c 0100 004d 4901  .TRP-CZ3r|...MI.
-000017b0: 5807 0000 0054 5250 2d43 4832 727d 0100  X....TRP-CH2r}..
-000017c0: 004d 4a01 5805 0000 0054 5250 2d48 727e  .MJ.X....TRP-Hr~
-000017d0: 0100 004d 4b01 5806 0000 0054 5250 2d48  ...MK.X....TRP-H
-000017e0: 4172 7f01 0000 4d4c 0158 0700 0000 5452  Ar....ML.X....TR
-000017f0: 502d 4842 3272 8001 0000 4d4d 0158 0700  P-HB2r....MM.X..
-00001800: 0000 5452 502d 4842 3372 8101 0000 4d4e  ..TRP-HB3r....MN
-00001810: 0158 0700 0000 5452 502d 4844 3172 8201  .X....TRP-HD1r..
-00001820: 0000 4d4f 0158 0700 0000 5452 502d 4845  ..MO.X....TRP-HE
-00001830: 3172 8301 0000 4d50 0158 0700 0000 5452  1r....MP.X....TR
-00001840: 502d 4845 3372 8401 0000 4d51 0158 0700  P-HE3r....MQ.X..
-00001850: 0000 5452 502d 485a 3272 8501 0000 4d52  ..TRP-HZ2r....MR
-00001860: 0158 0700 0000 5452 502d 485a 3372 8601  .X....TRP-HZ3r..
-00001870: 0000 4d53 0158 0700 0000 5452 502d 4848  ..MS.X....TRP-HH
-00001880: 3272 8701 0000 4d54 0158 0700 0000 474c  2r....MT.X....GL
-00001890: 592d 4f58 5472 8801 0000 4d55 0158 0600  Y-OXTr....MU.X..
-000018a0: 0000 5052 4f2d 4832 7289 0100 004d 5601  ..PRO-H2r....MV.
-000018b0: 5807 0000 0050 4845 2d4f 5854 728a 0100  X....PHE-OXTr...
-000018c0: 004d 5701 5807 0000 0047 4c4e 2d4f 5854  .MW.X....GLN-OXT
-000018d0: 728b 0100 004d 5801 5806 0000 0053 4552  r....MX.X....SER
-000018e0: 2d48 3272 8c01 0000 4d59 0158 0600 0000  -H2r....MY.X....
-000018f0: 5345 522d 4833 728d 0100 004d 5a01 5807  SER-H3r....MZ.X.
-00001900: 0000 0054 4852 2d4f 5854 728e 0100 004d  ...THR-OXTr....M
-00001910: 5b01 5807 0000 0047 4c55 2d4f 5854 728f  [.X....GLU-OXTr.
-00001920: 0100 004d 5c01 5806 0000 0047 4c59 2d48  ...M\.X....GLY-H
-00001930: 3272 9001 0000 4d5d 0158 0600 0000 474c  2r....M].X....GL
-00001940: 592d 4833 7291 0100 004d 5e01 5806 0000  Y-H3r....M^.X...
-00001950: 004d 4554 2d48 3272 9201 0000 4d5f 0158  .MET-H2r....M_.X
-00001960: 0600 0000 4d45 542d 4833 7293 0100 004d  ....MET-H3r....M
-00001970: 6001 5807 0000 0048 4953 2d4f 5854 7294  `.X....HIS-OXTr.
-00001980: 0100 004d 6101 5807 0000 0049 4c45 2d4f  ...Ma.X....ILE-O
-00001990: 5854 7295 0100 004d 6201 5806 0000 004c  XTr....Mb.X....L
-000019a0: 5953 2d48 3272 9601 0000 4d63 0158 0600  YS-H2r....Mc.X..
-000019b0: 0000 4c59 532d 4833 7297 0100 004d 6401  ..LYS-H3r....Md.
-000019c0: 5806 0000 0056 414c 2d48 3272 9801 0000  X....VAL-H2r....
-000019d0: 4d65 0158 0600 0000 5641 4c2d 4833 7299  Me.X....VAL-H3r.
-000019e0: 0100 004d 6601 5806 0000 0041 534e 2d48  ...Mf.X....ASN-H
-000019f0: 3272 9a01 0000 4d67 0158 0600 0000 4153  2r....Mg.X....AS
-00001a00: 4e2d 4833 729b 0100 004d 6801 5807 0000  N-H3r....Mh.X...
-00001a10: 0041 5247 2d4f 5854 729c 0100 004d 6901  .ARG-OXTr....Mi.
-00001a20: 5807 0000 0041 534e 2d4f 5854 729d 0100  X....ASN-OXTr...
-00001a30: 004d 6a01 5806 0000 0054 4852 2d48 3272  .Mj.X....THR-H2r
-00001a40: 9e01 0000 4d6b 0158 0600 0000 5448 522d  ....Mk.X....THR-
-00001a50: 4833 729f 0100 004d 6c01 5807 0000 0053  H3r....Ml.X....S
-00001a60: 4552 2d4f 5854 72a0 0100 004d 6d01 5807  ER-OXTr....Mm.X.
-00001a70: 0000 0050 524f 2d4f 5854 72a1 0100 004d  ...PRO-OXTr....M
-00001a80: 6e01 5806 0000 0050 4845 2d48 3272 a201  n.X....PHE-H2r..
-00001a90: 0000 4d6f 0158 0600 0000 5048 452d 4833  ..Mo.X....PHE-H3
-00001aa0: 72a3 0100 004d 7001 5807 0000 0053 4552  r....Mp.X....SER
-00001ab0: 2d48 5854 72a4 0100 004d 7101 5806 0000  -HXTr....Mq.X...
-00001ac0: 0041 5247 2d48 3272 a501 0000 4d72 0158  .ARG-H2r....Mr.X
-00001ad0: 0600 0000 4152 472d 4833 72a6 0100 004d  ....ARG-H3r....M
-00001ae0: 7301 5807 0000 004c 4555 2d4f 5854 72a7  s.X....LEU-OXTr.
-00001af0: 0100 004d 7401 5806 0000 0049 4c45 2d48  ...Mt.X....ILE-H
-00001b00: 3272 a801 0000 4d75 0158 0600 0000 494c  2r....Mu.X....IL
-00001b10: 452d 4833 72a9 0100 004d 7601 5806 0000  E-H3r....Mv.X...
-00001b20: 0047 4c4e 2d48 3272 aa01 0000 4d77 0158  .GLN-H2r....Mw.X
-00001b30: 0600 0000 474c 4e2d 4833 72ab 0100 004d  ....GLN-H3r....M
-00001b40: 7801 5807 0000 004c 5953 2d4f 5854 72ac  x.X....LYS-OXTr.
-00001b50: 0100 004d 7901 5806 0000 004c 4555 2d48  ...My.X....LEU-H
-00001b60: 3272 ad01 0000 4d7a 0158 0600 0000 4c45  2r....Mz.X....LE
-00001b70: 552d 4833 72ae 0100 004d 7b01 5806 0000  U-H3r....M{.X...
-00001b80: 0041 5350 2d48 3272 af01 0000 4d7c 0158  .ASP-H2r....M|.X
-00001b90: 0600 0000 4153 502d 4833 72b0 0100 004d  ....ASP-H3r....M
-00001ba0: 7d01 5807 0000 0056 414c 2d4f 5854 72b1  }.X....VAL-OXTr.
-00001bb0: 0100 004d 7e01 5807 0000 0054 5250 2d4f  ...M~.X....TRP-O
-00001bc0: 5854 72b2 0100 004d 7f01 5806 0000 0047  XTr....M..X....G
-00001bd0: 4c55 2d48 3272 b301 0000 4d80 0158 0600  LU-H2r....M..X..
-00001be0: 0000 474c 552d 4833 72b4 0100 004d 8101  ..GLU-H3r....M..
-00001bf0: 5807 0000 0043 5953 2d4f 5854 72b5 0100  X....CYS-OXTr...
-00001c00: 004d 8201 5807 0000 0041 5350 2d4f 5854  .M..X....ASP-OXT
-00001c10: 72b6 0100 004d 8301 5807 0000 0054 5952  r....M..X....TYR
-00001c20: 2d4f 5854 72b7 0100 004d 8401 5806 0000  -OXTr....M..X...
-00001c30: 0043 5953 2d48 3272 b801 0000 4d85 0158  .CYS-H2r....M..X
-00001c40: 0600 0000 4359 532d 4833 72b9 0100 004d  ....CYS-H3r....M
-00001c50: 8601 5806 0000 0054 5952 2d48 3272 ba01  ..X....TYR-H2r..
-00001c60: 0000 4d87 0158 0600 0000 5459 522d 4833  ..M..X....TYR-H3
-00001c70: 72bb 0100 004d 8801 5806 0000 0054 5250  r....M..X....TRP
-00001c80: 2d48 3272 bc01 0000 4d89 0158 0600 0000  -H2r....M..X....
-00001c90: 5452 502d 4833 72bd 0100 004d 8a01 5807  TRP-H3r....M..X.
-00001ca0: 0000 004d 4554 2d4f 5854 72be 0100 004d  ...MET-OXTr....M
-00001cb0: 8b01 5806 0000 0041 4c41 2d44 3172 bf01  ..X....ALA-D1r..
-00001cc0: 0000 4d8c 0158 0700 0000 5452 502d 4445  ..M..X....TRP-DE
-00001cd0: 3172 c001 0000 4d8d 0158 0600 0000 5459  1r....M..X....TY
-00001ce0: 522d 4448 72c1 0100 004d 8e01 5808 0000  R-DHr....M..X...
-00001cf0: 0041 534e 2d44 4432 3172 c201 0000 4d8f  .ASN-DD21r....M.
-00001d00: 0158 0600 0000 5345 522d 4447 72c3 0100  .X....SER-DGr...
-00001d10: 004d 9001 5807 0000 0054 4852 2d44 4731  .M..X....THR-DG1
-00001d20: 72c4 0100 004d 9101 5807 0000 004c 5953  r....M..X....LYS
-00001d30: 2d44 5a31 72c5 0100 004d 9201 5806 0000  -DZ1r....M..X...
-00001d40: 0048 4953 2d48 3272 c601 0000 4d93 0158  .HIS-H2r....M..X
-00001d50: 0600 0000 4849 532d 4833 72c7 0100 004d  ....HIS-H3r....M
-00001d60: 9401 5806 0000 0056 414c 2d44 3172 c801  ..X....VAL-D1r..
-00001d70: 0000 4d95 0158 0500 0000 4c45 552d 4472  ..M..X....LEU-Dr
-00001d80: c901 0000 4d96 0158 0500 0000 5345 522d  ....M..X....SER-
-00001d90: 4472 ca01 0000 4d97 0158 0500 0000 474c  Dr....M..X....GL
-00001da0: 552d 4472 cb01 0000 4d98 0158 0500 0000  U-Dr....M..X....
-00001db0: 5452 502d 4472 cc01 0000 4d99 0158 0500  TRP-Dr....M..X..
-00001dc0: 0000 474c 4e2d 4472 cd01 0000 4d9a 0158  ..GLN-Dr....M..X
-00001dd0: 0500 0000 414c 412d 4472 ce01 0000 4d9b  ....ALA-Dr....M.
-00001de0: 0158 0500 0000 5641 4c2d 4472 cf01 0000  .X....VAL-Dr....
-00001df0: 4d9c 0158 0500 0000 4153 502d 4472 d001  M..X....ASP-Dr..
-00001e00: 0000 4d9d 0158 0500 0000 474c 592d 4472  ..M..X....GLY-Dr
-00001e10: d101 0000 4d9e 0158 0500 0000 5048 452d  ....M..X....PHE-
-00001e20: 4472 d201 0000 4d9f 0158 0500 0000 4c59  Dr....M..X....LY
-00001e30: 532d 4472 d301 0000 4da0 0158 0500 0000  S-Dr....M..X....
-00001e40: 4849 532d 4472 d401 0000 4da1 0158 0500  HIS-Dr....M..X..
-00001e50: 0000 4152 472d 4472 d501 0000 4da2 0158  ..ARG-Dr....M..X
-00001e60: 0500 0000 5448 522d 4472 d601 0000 4da3  ....THR-Dr....M.
-00001e70: 0158 0500 0000 494c 452d 4472 d701 0000  .X....ILE-Dr....
-00001e80: 4da4 0158 0700 0000 414c 412d 4858 5472  M..X....ALA-HXTr
-00001e90: d801 0000 4da5 0158 0700 0000 4152 472d  ....M..X....ARG-
-00001ea0: 4858 5472 d901 0000 4da6 0158 0500 0000  HXTr....M..X....
-00001eb0: 5459 522d 4472 da01 0000 4da7 0158 0700  TYR-Dr....M..X..
-00001ec0: 0000 4c59 532d 445a 3372 db01 0000 4da8  ..LYS-DZ3r....M.
-00001ed0: 0158 0700 0000 4c59 532d 445a 3272 dc01  .X....LYS-DZ2r..
-00001ee0: 0000 4da9 0158 0700 0000 4849 532d 4445  ..M..X....HIS-DE
-00001ef0: 3272 dd01 0000 4daa 0158 0700 0000 4849  2r....M..X....HI
-00001f00: 532d 4444 3172 de01 0000 4dab 0158 0600  S-DD1r....M..X..
-00001f10: 0000 4152 472d 4445 72df 0100 004d ac01  ..ARG-DEr....M..
-00001f20: 5805 0000 004d 4554 2d44 72e0 0100 004d  X....MET-Dr....M
-00001f30: ad01 5808 0000 0041 5247 2d44 4831 3172  ..X....ARG-DH11r
-00001f40: e101 0000 4dae 0158 0600 0000 414c 412d  ....M..X....ALA-
-00001f50: 4432 72e2 0100 004d af01 5805 0000 0044  D2r....M..X....D
-00001f60: 4654 2d4f 72e3 0100 004d b001 5805 0000  FT-Or....M..X...
-00001f70: 0044 4654 2d43 72e4 0100 004d b101 5805  .DFT-Cr....M..X.
-00001f80: 0000 0044 4654 2d48 72e5 0100 004d b201  ...DFT-Hr....M..
-00001f90: 5805 0000 0044 4654 2d4e 72e6 0100 004d  X....DFT-Nr....M
-00001fa0: b301 7575 2e                             ..uu.
+00000070: 0200 0000 436c 710c 4b09 5801 0000 0046  ....Clq.K.X....F
+00000080: 710d 4b0a 7558 0400 0000 626f 6e64 710e  q.K.uX....bondq.
+00000090: 7d71 0f28 5804 0000 006e 6f6e 6571 104b  }q.(X....noneq.K
+000000a0: 0058 0600 0000 7369 6e67 6c65 7111 4b01  .X....singleq.K.
+000000b0: 5806 0000 0064 6f75 626c 6571 124b 0258  X....doubleq.K.X
+000000c0: 0600 0000 7472 6970 6c65 7113 4b03 5808  ....tripleq.K.X.
+000000d0: 0000 0061 726f 6d61 7469 6371 144b 0475  ...aromaticq.K.u
+000000e0: 5803 0000 0065 7870 7115 7d71 1658 0000  X....expq.}q.X..
+000000f0: 0000 7117 4b00 7358 0500 0000 6e6c 6973  ..q.K.sX....nlis
+00000100: 7471 187d 7119 2868 104b 0058 0900 0000  tq.}q.(h.K.X....
+00000110: 6e6f 6e62 6f6e 6465 6471 1a4b 014b 014b  nonbondedq.K.K.K
+00000120: 024b 024b 034b 034b 044b 044b 054b 054b  .K.K.K.K.K.K.K.K
+00000130: 064b 064b 0775 5805 0000 0063 6c61 7373  .K.K.uX....class
+00000140: 711b 7d71 1c28 5803 0000 0041 4c41 711d  q.}q.(X....ALAq.
+00000150: 4b00 5803 0000 0041 5247 711e 4b01 5803  K.X....ARGq.K.X.
+00000160: 0000 0041 534e 711f 4b02 5803 0000 0041  ...ASNq.K.X....A
+00000170: 5350 7120 4b03 5803 0000 0043 5953 7121  SPq K.X....CYSq!
+00000180: 4b04 5803 0000 0047 4c55 7122 4b05 5803  K.X....GLUq"K.X.
+00000190: 0000 0047 4c4e 7123 4b06 5803 0000 0047  ...GLNq#K.X....G
+000001a0: 4c59 7124 4b07 5803 0000 0048 4953 7125  LYq$K.X....HISq%
+000001b0: 4b08 5803 0000 0049 4c45 7126 4b09 5803  K.X....ILEq&K.X.
+000001c0: 0000 004c 4555 7127 4b0a 5803 0000 004c  ...LEUq'K.X....L
+000001d0: 5953 7128 4b0b 5803 0000 004d 4554 7129  YSq(K.X....METq)
+000001e0: 4b0c 5803 0000 0050 4845 712a 4b0d 5803  K.X....PHEq*K.X.
+000001f0: 0000 0050 524f 712b 4b0e 5803 0000 0053  ...PROq+K.X....S
+00000200: 4552 712c 4b0f 5803 0000 0054 4852 712d  ERq,K.X....THRq-
+00000210: 4b10 5803 0000 0054 5250 712e 4b11 5803  K.X....TRPq.K.X.
+00000220: 0000 0054 5952 712f 4b12 5803 0000 0056  ...TYRq/K.X....V
+00000230: 414c 7130 4b13 5802 0000 004d 4271 314b  ALq0K.X....MBq1K
+00000240: 1458 0300 0000 4446 5471 324b 1558 0300  .X....DFTq2K.X..
+00000250: 0000 4341 5371 334b 1675 5804 0000 006e  ..CASq3K.uX....n
+00000260: 616d 6571 347d 7135 2868 034b 0058 0400  ameq4}q5(h.K.X..
+00000270: 0000 4d42 2d4e 7136 4b01 5804 0000 004d  ..MB-Nq6K.X....M
+00000280: 422d 4371 374b 0258 0400 0000 4d42 2d48  B-Cq7K.X....MB-H
+00000290: 7138 4b03 5804 0000 004d 422d 4f71 394b  q8K.X....MB-Oq9K
+000002a0: 0458 0400 0000 4d42 2d53 713a 4b05 5804  .X....MB-Sq:K.X.
+000002b0: 0000 004d 422d 5071 3b4b 0658 0400 0000  ...MB-Pq;K.X....
+000002c0: 4d42 2d49 713c 4b07 5805 0000 004d 422d  MB-Iq<K.X....MB-
+000002d0: 436c 713d 4b08 5805 0000 0050 524f 2d4e  Clq=K.X....PRO-N
+000002e0: 713e 4b09 5806 0000 0050 524f 2d43 4171  q>K.X....PRO-CAq
+000002f0: 3f4b 0a58 0500 0000 5052 4f2d 4371 404b  ?K.X....PRO-Cq@K
+00000300: 0b58 0500 0000 5052 4f2d 4f71 414b 0c58  .X....PRO-OqAK.X
+00000310: 0600 0000 5052 4f2d 4342 7142 4b0d 5806  ....PRO-CBqBK.X.
+00000320: 0000 0050 524f 2d43 4771 434b 0e58 0600  ...PRO-CGqCK.X..
+00000330: 0000 5052 4f2d 4344 7144 4b0f 5805 0000  ..PRO-CDqDK.X...
+00000340: 0050 524f 2d48 7145 4b10 5806 0000 0050  .PRO-HqEK.X....P
+00000350: 524f 2d48 3371 464b 1158 0600 0000 5052  RO-H3qFK.X....PR
+00000360: 4f2d 4841 7147 4b12 5807 0000 0050 524f  O-HAqGK.X....PRO
+00000370: 2d48 4232 7148 4b13 5807 0000 0050 524f  -HB2qHK.X....PRO
+00000380: 2d48 4233 7149 4b14 5807 0000 0050 524f  -HB3qIK.X....PRO
+00000390: 2d48 4732 714a 4b15 5807 0000 0050 524f  -HG2qJK.X....PRO
+000003a0: 2d48 4733 714b 4b16 5807 0000 0050 524f  -HG3qKK.X....PRO
+000003b0: 2d48 4432 714c 4b17 5807 0000 0050 524f  -HD2qLK.X....PRO
+000003c0: 2d48 4433 714d 4b18 5805 0000 0049 4c45  -HD3qMK.X....ILE
+000003d0: 2d4e 714e 4b19 5806 0000 0049 4c45 2d43  -NqNK.X....ILE-C
+000003e0: 4171 4f4b 1a58 0500 0000 494c 452d 4371  AqOK.X....ILE-Cq
+000003f0: 504b 1b58 0500 0000 494c 452d 4f71 514b  PK.X....ILE-OqQK
+00000400: 1c58 0600 0000 494c 452d 4342 7152 4b1d  .X....ILE-CBqRK.
+00000410: 5807 0000 0049 4c45 2d43 4731 7153 4b1e  X....ILE-CG1qSK.
+00000420: 5807 0000 0049 4c45 2d43 4732 7154 4b1f  X....ILE-CG2qTK.
+00000430: 5807 0000 0049 4c45 2d43 4431 7155 4b20  X....ILE-CD1qUK 
+00000440: 5805 0000 0049 4c45 2d48 7156 4b21 5806  X....ILE-HqVK!X.
+00000450: 0000 0049 4c45 2d48 4171 574b 2258 0600  ...ILE-HAqWK"X..
+00000460: 0000 494c 452d 4842 7158 4b23 5808 0000  ..ILE-HBqXK#X...
+00000470: 0049 4c45 2d48 4731 3271 594b 2458 0800  .ILE-HG12qYK$X..
+00000480: 0000 494c 452d 4847 3133 715a 4b25 5808  ..ILE-HG13qZK%X.
+00000490: 0000 0049 4c45 2d48 4732 3171 5b4b 2658  ...ILE-HG21q[K&X
+000004a0: 0800 0000 494c 452d 4847 3232 715c 4b27  ....ILE-HG22q\K'
+000004b0: 5808 0000 0049 4c45 2d48 4732 3371 5d4b  X....ILE-HG23q]K
+000004c0: 2858 0800 0000 494c 452d 4844 3131 715e  (X....ILE-HD11q^
+000004d0: 4b29 5808 0000 0049 4c45 2d48 4431 3271  K)X....ILE-HD12q
+000004e0: 5f4b 2a58 0800 0000 494c 452d 4844 3133  _K*X....ILE-HD13
+000004f0: 7160 4b2b 5805 0000 0056 414c 2d4e 7161  q`K+X....VAL-Nqa
+00000500: 4b2c 5806 0000 0056 414c 2d43 4171 624b  K,X....VAL-CAqbK
+00000510: 2d58 0500 0000 5641 4c2d 4371 634b 2e58  -X....VAL-CqcK.X
+00000520: 0500 0000 5641 4c2d 4f71 644b 2f58 0600  ....VAL-OqdK/X..
+00000530: 0000 5641 4c2d 4342 7165 4b30 5807 0000  ..VAL-CBqeK0X...
+00000540: 0056 414c 2d43 4731 7166 4b31 5807 0000  .VAL-CG1qfK1X...
+00000550: 0056 414c 2d43 4732 7167 4b32 5805 0000  .VAL-CG2qgK2X...
+00000560: 0056 414c 2d48 7168 4b33 5806 0000 0056  .VAL-HqhK3X....V
+00000570: 414c 2d48 4171 694b 3458 0600 0000 5641  AL-HAqiK4X....VA
+00000580: 4c2d 4842 716a 4b35 5808 0000 0056 414c  L-HBqjK5X....VAL
+00000590: 2d48 4731 3171 6b4b 3658 0800 0000 5641  -HG11qkK6X....VA
+000005a0: 4c2d 4847 3132 716c 4b37 5808 0000 0056  L-HG12qlK7X....V
+000005b0: 414c 2d48 4731 3371 6d4b 3858 0800 0000  AL-HG13qmK8X....
+000005c0: 5641 4c2d 4847 3231 716e 4b39 5808 0000  VAL-HG21qnK9X...
+000005d0: 0056 414c 2d48 4732 3271 6f4b 3a58 0800  .VAL-HG22qoK:X..
+000005e0: 0000 5641 4c2d 4847 3233 7170 4b3b 5805  ..VAL-HG23qpK;X.
+000005f0: 0000 0041 5247 2d4e 7171 4b3c 5806 0000  ...ARG-NqqK<X...
+00000600: 0041 5247 2d43 4171 724b 3d58 0500 0000  .ARG-CAqrK=X....
+00000610: 4152 472d 4371 734b 3e58 0500 0000 4152  ARG-CqsK>X....AR
+00000620: 472d 4f71 744b 3f58 0600 0000 4152 472d  G-OqtK?X....ARG-
+00000630: 4342 7175 4b40 5806 0000 0041 5247 2d43  CBquK@X....ARG-C
+00000640: 4771 764b 4158 0600 0000 4152 472d 4344  GqvKAX....ARG-CD
+00000650: 7177 4b42 5806 0000 0041 5247 2d4e 4571  qwKBX....ARG-NEq
+00000660: 784b 4358 0600 0000 4152 472d 435a 7179  xKCX....ARG-CZqy
+00000670: 4b44 5807 0000 0041 5247 2d4e 4831 717a  KDX....ARG-NH1qz
+00000680: 4b45 5807 0000 0041 5247 2d4e 4832 717b  KEX....ARG-NH2q{
+00000690: 4b46 5805 0000 0041 5247 2d48 717c 4b47  KFX....ARG-Hq|KG
+000006a0: 5806 0000 0041 5247 2d48 4171 7d4b 4858  X....ARG-HAq}KHX
+000006b0: 0700 0000 4152 472d 4842 3271 7e4b 4958  ....ARG-HB2q~KIX
+000006c0: 0700 0000 4152 472d 4842 3371 7f4b 4a58  ....ARG-HB3q.KJX
+000006d0: 0700 0000 4152 472d 4847 3271 804b 4b58  ....ARG-HG2q.KKX
+000006e0: 0700 0000 4152 472d 4847 3371 814b 4c58  ....ARG-HG3q.KLX
+000006f0: 0700 0000 4152 472d 4844 3271 824b 4d58  ....ARG-HD2q.KMX
+00000700: 0700 0000 4152 472d 4844 3371 834b 4e58  ....ARG-HD3q.KNX
+00000710: 0600 0000 4152 472d 4845 7184 4b4f 5808  ....ARG-HEq.KOX.
+00000720: 0000 0041 5247 2d48 4831 3171 854b 5058  ...ARG-HH11q.KPX
+00000730: 0800 0000 4152 472d 4848 3132 7186 4b51  ....ARG-HH12q.KQ
+00000740: 5808 0000 0041 5247 2d48 4832 3171 874b  X....ARG-HH21q.K
+00000750: 5258 0800 0000 4152 472d 4848 3232 7188  RX....ARG-HH22q.
+00000760: 4b53 5805 0000 004c 5953 2d4e 7189 4b54  KSX....LYS-Nq.KT
+00000770: 5806 0000 004c 5953 2d43 4171 8a4b 5558  X....LYS-CAq.KUX
+00000780: 0500 0000 4c59 532d 4371 8b4b 5658 0500  ....LYS-Cq.KVX..
+00000790: 0000 4c59 532d 4f71 8c4b 5758 0600 0000  ..LYS-Oq.KWX....
+000007a0: 4c59 532d 4342 718d 4b58 5806 0000 004c  LYS-CBq.KXX....L
+000007b0: 5953 2d43 4771 8e4b 5958 0600 0000 4c59  YS-CGq.KYX....LY
+000007c0: 532d 4344 718f 4b5a 5806 0000 004c 5953  S-CDq.KZX....LYS
+000007d0: 2d43 4571 904b 5b58 0600 0000 4c59 532d  -CEq.K[X....LYS-
+000007e0: 4e5a 7191 4b5c 5805 0000 004c 5953 2d48  NZq.K\X....LYS-H
+000007f0: 7192 4b5d 5806 0000 004c 5953 2d48 4171  q.K]X....LYS-HAq
+00000800: 934b 5e58 0700 0000 4c59 532d 4842 3271  .K^X....LYS-HB2q
+00000810: 944b 5f58 0700 0000 4c59 532d 4842 3371  .K_X....LYS-HB3q
+00000820: 954b 6058 0700 0000 4c59 532d 4847 3271  .K`X....LYS-HG2q
+00000830: 964b 6158 0700 0000 4c59 532d 4847 3371  .KaX....LYS-HG3q
+00000840: 974b 6258 0700 0000 4c59 532d 4844 3271  .KbX....LYS-HD2q
+00000850: 984b 6358 0700 0000 4c59 532d 4844 3371  .KcX....LYS-HD3q
+00000860: 994b 6458 0700 0000 4c59 532d 4845 3271  .KdX....LYS-HE2q
+00000870: 9a4b 6558 0700 0000 4c59 532d 4845 3371  .KeX....LYS-HE3q
+00000880: 9b4b 6658 0700 0000 4c59 532d 485a 3171  .KfX....LYS-HZ1q
+00000890: 9c4b 6758 0700 0000 4c59 532d 485a 3271  .KgX....LYS-HZ2q
+000008a0: 9d4b 6858 0700 0000 4c59 532d 485a 3371  .KhX....LYS-HZ3q
+000008b0: 9e4b 6958 0500 0000 474c 552d 4e71 9f4b  .KiX....GLU-Nq.K
+000008c0: 6a58 0600 0000 474c 552d 4341 71a0 4b6b  jX....GLU-CAq.Kk
+000008d0: 5805 0000 0047 4c55 2d43 71a1 4b6c 5805  X....GLU-Cq.KlX.
+000008e0: 0000 0047 4c55 2d4f 71a2 4b6d 5806 0000  ...GLU-Oq.KmX...
+000008f0: 0047 4c55 2d43 4271 a34b 6e58 0600 0000  .GLU-CBq.KnX....
+00000900: 474c 552d 4347 71a4 4b6f 5806 0000 0047  GLU-CGq.KoX....G
+00000910: 4c55 2d43 4471 a54b 7058 0700 0000 474c  LU-CDq.KpX....GL
+00000920: 552d 4f45 3171 a64b 7158 0700 0000 474c  U-OE1q.KqX....GL
+00000930: 552d 4f45 3271 a74b 7258 0500 0000 474c  U-OE2q.KrX....GL
+00000940: 552d 4871 a84b 7358 0600 0000 474c 552d  U-Hq.KsX....GLU-
+00000950: 4841 71a9 4b74 5807 0000 0047 4c55 2d48  HAq.KtX....GLU-H
+00000960: 4232 71aa 4b75 5807 0000 0047 4c55 2d48  B2q.KuX....GLU-H
+00000970: 4233 71ab 4b76 5807 0000 0047 4c55 2d48  B3q.KvX....GLU-H
+00000980: 4732 71ac 4b77 5807 0000 0047 4c55 2d48  G2q.KwX....GLU-H
+00000990: 4733 71ad 4b78 5805 0000 004c 4555 2d4e  G3q.KxX....LEU-N
+000009a0: 71ae 4b79 5806 0000 004c 4555 2d43 4171  q.KyX....LEU-CAq
+000009b0: af4b 7a58 0500 0000 4c45 552d 4371 b04b  .KzX....LEU-Cq.K
+000009c0: 7b58 0500 0000 4c45 552d 4f71 b14b 7c58  {X....LEU-Oq.K|X
+000009d0: 0600 0000 4c45 552d 4342 71b2 4b7d 5806  ....LEU-CBq.K}X.
+000009e0: 0000 004c 4555 2d43 4771 b34b 7e58 0700  ...LEU-CGq.K~X..
+000009f0: 0000 4c45 552d 4344 3171 b44b 7f58 0700  ..LEU-CD1q.K.X..
+00000a00: 0000 4c45 552d 4344 3271 b54b 8058 0500  ..LEU-CD2q.K.X..
+00000a10: 0000 4c45 552d 4871 b64b 8158 0600 0000  ..LEU-Hq.K.X....
+00000a20: 4c45 552d 4841 71b7 4b82 5807 0000 004c  LEU-HAq.K.X....L
+00000a30: 4555 2d48 4232 71b8 4b83 5807 0000 004c  EU-HB2q.K.X....L
+00000a40: 4555 2d48 4233 71b9 4b84 5806 0000 004c  EU-HB3q.K.X....L
+00000a50: 4555 2d48 4771 ba4b 8558 0800 0000 4c45  EU-HGq.K.X....LE
+00000a60: 552d 4844 3131 71bb 4b86 5808 0000 004c  U-HD11q.K.X....L
+00000a70: 4555 2d48 4431 3271 bc4b 8758 0800 0000  EU-HD12q.K.X....
+00000a80: 4c45 552d 4844 3133 71bd 4b88 5808 0000  LEU-HD13q.K.X...
+00000a90: 004c 4555 2d48 4432 3171 be4b 8958 0800  .LEU-HD21q.K.X..
+00000aa0: 0000 4c45 552d 4844 3232 71bf 4b8a 5808  ..LEU-HD22q.K.X.
+00000ab0: 0000 004c 4555 2d48 4432 3371 c04b 8b58  ...LEU-HD23q.K.X
+00000ac0: 0500 0000 5459 522d 4e71 c14b 8c58 0600  ....TYR-Nq.K.X..
+00000ad0: 0000 5459 522d 4341 71c2 4b8d 5805 0000  ..TYR-CAq.K.X...
+00000ae0: 0054 5952 2d43 71c3 4b8e 5805 0000 0054  .TYR-Cq.K.X....T
+00000af0: 5952 2d4f 71c4 4b8f 5806 0000 0054 5952  YR-Oq.K.X....TYR
+00000b00: 2d43 4271 c54b 9058 0600 0000 5459 522d  -CBq.K.X....TYR-
+00000b10: 4347 71c6 4b91 5807 0000 0054 5952 2d43  CGq.K.X....TYR-C
+00000b20: 4431 71c7 4b92 5807 0000 0054 5952 2d43  D1q.K.X....TYR-C
+00000b30: 4432 71c8 4b93 5807 0000 0054 5952 2d43  D2q.K.X....TYR-C
+00000b40: 4531 71c9 4b94 5807 0000 0054 5952 2d43  E1q.K.X....TYR-C
+00000b50: 4532 71ca 4b95 5806 0000 0054 5952 2d43  E2q.K.X....TYR-C
+00000b60: 5a71 cb4b 9658 0600 0000 5459 522d 4f48  Zq.K.X....TYR-OH
+00000b70: 71cc 4b97 5805 0000 0054 5952 2d48 71cd  q.K.X....TYR-Hq.
+00000b80: 4b98 5806 0000 0054 5952 2d48 4171 ce4b  K.X....TYR-HAq.K
+00000b90: 9958 0700 0000 5459 522d 4842 3271 cf4b  .X....TYR-HB2q.K
+00000ba0: 9a58 0700 0000 5459 522d 4842 3371 d04b  .X....TYR-HB3q.K
+00000bb0: 9b58 0700 0000 5459 522d 4844 3171 d14b  .X....TYR-HD1q.K
+00000bc0: 9c58 0700 0000 5459 522d 4844 3271 d24b  .X....TYR-HD2q.K
+00000bd0: 9d58 0700 0000 5459 522d 4845 3171 d34b  .X....TYR-HE1q.K
+00000be0: 9e58 0700 0000 5459 522d 4845 3271 d44b  .X....TYR-HE2q.K
+00000bf0: 9f58 0600 0000 5459 522d 4848 71d5 4ba0  .X....TYR-HHq.K.
+00000c00: 5805 0000 0043 5953 2d4e 71d6 4ba1 5806  X....CYS-Nq.K.X.
+00000c10: 0000 0043 5953 2d43 4171 d74b a258 0500  ...CYS-CAq.K.X..
+00000c20: 0000 4359 532d 4371 d84b a358 0500 0000  ..CYS-Cq.K.X....
+00000c30: 4359 532d 4f71 d94b a458 0600 0000 4359  CYS-Oq.K.X....CY
+00000c40: 532d 4342 71da 4ba5 5806 0000 0043 5953  S-CBq.K.X....CYS
+00000c50: 2d53 4771 db4b a658 0500 0000 4359 532d  -SGq.K.X....CYS-
+00000c60: 4871 dc4b a758 0600 0000 4359 532d 4841  Hq.K.X....CYS-HA
+00000c70: 71dd 4ba8 5807 0000 0043 5953 2d48 4232  q.K.X....CYS-HB2
+00000c80: 71de 4ba9 5807 0000 0043 5953 2d48 4233  q.K.X....CYS-HB3
+00000c90: 71df 4baa 5806 0000 0043 5953 2d48 4771  q.K.X....CYS-HGq
+00000ca0: e04b ab58 0500 0000 474c 592d 4e71 e14b  .K.X....GLY-Nq.K
+00000cb0: ac58 0600 0000 474c 592d 4341 71e2 4bad  .X....GLY-CAq.K.
+00000cc0: 5805 0000 0047 4c59 2d43 71e3 4bae 5805  X....GLY-Cq.K.X.
+00000cd0: 0000 0047 4c59 2d4f 71e4 4baf 5805 0000  ...GLY-Oq.K.X...
+00000ce0: 0047 4c59 2d48 71e5 4bb0 5807 0000 0047  .GLY-Hq.K.X....G
+00000cf0: 4c59 2d48 4132 71e6 4bb1 5807 0000 0047  LY-HA2q.K.X....G
+00000d00: 4c59 2d48 4133 71e7 4bb2 5805 0000 0050  LY-HA3q.K.X....P
+00000d10: 4845 2d4e 71e8 4bb3 5806 0000 0050 4845  HE-Nq.K.X....PHE
+00000d20: 2d43 4171 e94b b458 0500 0000 5048 452d  -CAq.K.X....PHE-
+00000d30: 4371 ea4b b558 0500 0000 5048 452d 4f71  Cq.K.X....PHE-Oq
+00000d40: eb4b b658 0600 0000 5048 452d 4342 71ec  .K.X....PHE-CBq.
+00000d50: 4bb7 5806 0000 0050 4845 2d43 4771 ed4b  K.X....PHE-CGq.K
+00000d60: b858 0700 0000 5048 452d 4344 3171 ee4b  .X....PHE-CD1q.K
+00000d70: b958 0700 0000 5048 452d 4344 3271 ef4b  .X....PHE-CD2q.K
+00000d80: ba58 0700 0000 5048 452d 4345 3171 f04b  .X....PHE-CE1q.K
+00000d90: bb58 0700 0000 5048 452d 4345 3271 f14b  .X....PHE-CE2q.K
+00000da0: bc58 0600 0000 5048 452d 435a 71f2 4bbd  .X....PHE-CZq.K.
+00000db0: 5805 0000 0050 4845 2d48 71f3 4bbe 5806  X....PHE-Hq.K.X.
+00000dc0: 0000 0050 4845 2d48 4171 f44b bf58 0700  ...PHE-HAq.K.X..
+00000dd0: 0000 5048 452d 4842 3271 f54b c058 0700  ..PHE-HB2q.K.X..
+00000de0: 0000 5048 452d 4842 3371 f64b c158 0700  ..PHE-HB3q.K.X..
+00000df0: 0000 5048 452d 4844 3171 f74b c258 0700  ..PHE-HD1q.K.X..
+00000e00: 0000 5048 452d 4844 3271 f84b c358 0700  ..PHE-HD2q.K.X..
+00000e10: 0000 5048 452d 4845 3171 f94b c458 0700  ..PHE-HE1q.K.X..
+00000e20: 0000 5048 452d 4845 3271 fa4b c558 0600  ..PHE-HE2q.K.X..
+00000e30: 0000 5048 452d 485a 71fb 4bc6 5805 0000  ..PHE-HZq.K.X...
+00000e40: 0041 4c41 2d4e 71fc 4bc7 5806 0000 0041  .ALA-Nq.K.X....A
+00000e50: 4c41 2d43 4171 fd4b c858 0500 0000 414c  LA-CAq.K.X....AL
+00000e60: 412d 4371 fe4b c958 0500 0000 414c 412d  A-Cq.K.X....ALA-
+00000e70: 4f71 ff4b ca58 0600 0000 414c 412d 4342  Oq.K.X....ALA-CB
+00000e80: 7200 0100 004b cb58 0500 0000 414c 412d  r....K.X....ALA-
+00000e90: 4872 0101 0000 4bcc 5806 0000 0041 4c41  Hr....K.X....ALA
+00000ea0: 2d48 4172 0201 0000 4bcd 5807 0000 0041  -HAr....K.X....A
+00000eb0: 4c41 2d48 4231 7203 0100 004b ce58 0700  LA-HB1r....K.X..
+00000ec0: 0000 414c 412d 4842 3272 0401 0000 4bcf  ..ALA-HB2r....K.
+00000ed0: 5807 0000 0041 4c41 2d48 4233 7205 0100  X....ALA-HB3r...
+00000ee0: 004b d058 0500 0000 474c 4e2d 4e72 0601  .K.X....GLN-Nr..
+00000ef0: 0000 4bd1 5806 0000 0047 4c4e 2d43 4172  ..K.X....GLN-CAr
+00000f00: 0701 0000 4bd2 5805 0000 0047 4c4e 2d43  ....K.X....GLN-C
+00000f10: 7208 0100 004b d358 0500 0000 474c 4e2d  r....K.X....GLN-
+00000f20: 4f72 0901 0000 4bd4 5806 0000 0047 4c4e  Or....K.X....GLN
+00000f30: 2d43 4272 0a01 0000 4bd5 5806 0000 0047  -CBr....K.X....G
+00000f40: 4c4e 2d43 4772 0b01 0000 4bd6 5806 0000  LN-CGr....K.X...
+00000f50: 0047 4c4e 2d43 4472 0c01 0000 4bd7 5807  .GLN-CDr....K.X.
+00000f60: 0000 0047 4c4e 2d4f 4531 720d 0100 004b  ...GLN-OE1r....K
+00000f70: d858 0700 0000 474c 4e2d 4e45 3272 0e01  .X....GLN-NE2r..
+00000f80: 0000 4bd9 5805 0000 0047 4c4e 2d48 720f  ..K.X....GLN-Hr.
+00000f90: 0100 004b da58 0600 0000 474c 4e2d 4841  ...K.X....GLN-HA
+00000fa0: 7210 0100 004b db58 0700 0000 474c 4e2d  r....K.X....GLN-
+00000fb0: 4842 3272 1101 0000 4bdc 5807 0000 0047  HB2r....K.X....G
+00000fc0: 4c4e 2d48 4233 7212 0100 004b dd58 0700  LN-HB3r....K.X..
+00000fd0: 0000 474c 4e2d 4847 3272 1301 0000 4bde  ..GLN-HG2r....K.
+00000fe0: 5807 0000 0047 4c4e 2d48 4733 7214 0100  X....GLN-HG3r...
+00000ff0: 004b df58 0800 0000 474c 4e2d 4845 3231  .K.X....GLN-HE21
+00001000: 7215 0100 004b e058 0800 0000 474c 4e2d  r....K.X....GLN-
+00001010: 4845 3232 7216 0100 004b e158 0500 0000  HE22r....K.X....
+00001020: 4153 502d 4e72 1701 0000 4be2 5806 0000  ASP-Nr....K.X...
+00001030: 0041 5350 2d43 4172 1801 0000 4be3 5805  .ASP-CAr....K.X.
+00001040: 0000 0041 5350 2d43 7219 0100 004b e458  ...ASP-Cr....K.X
+00001050: 0500 0000 4153 502d 4f72 1a01 0000 4be5  ....ASP-Or....K.
+00001060: 5806 0000 0041 5350 2d43 4272 1b01 0000  X....ASP-CBr....
+00001070: 4be6 5806 0000 0041 5350 2d43 4772 1c01  K.X....ASP-CGr..
+00001080: 0000 4be7 5807 0000 0041 5350 2d4f 4431  ..K.X....ASP-OD1
+00001090: 721d 0100 004b e858 0700 0000 4153 502d  r....K.X....ASP-
+000010a0: 4f44 3272 1e01 0000 4be9 5805 0000 0041  OD2r....K.X....A
+000010b0: 5350 2d48 721f 0100 004b ea58 0600 0000  SP-Hr....K.X....
+000010c0: 4153 502d 4841 7220 0100 004b eb58 0700  ASP-HAr ...K.X..
+000010d0: 0000 4153 502d 4842 3272 2101 0000 4bec  ..ASP-HB2r!...K.
+000010e0: 5807 0000 0041 5350 2d48 4233 7222 0100  X....ASP-HB3r"..
+000010f0: 004b ed58 0500 0000 4849 532d 4e72 2301  .K.X....HIS-Nr#.
+00001100: 0000 4bee 5806 0000 0048 4953 2d43 4172  ..K.X....HIS-CAr
+00001110: 2401 0000 4bef 5805 0000 0048 4953 2d43  $...K.X....HIS-C
+00001120: 7225 0100 004b f058 0500 0000 4849 532d  r%...K.X....HIS-
+00001130: 4f72 2601 0000 4bf1 5806 0000 0048 4953  Or&...K.X....HIS
+00001140: 2d43 4272 2701 0000 4bf2 5806 0000 0048  -CBr'...K.X....H
+00001150: 4953 2d43 4772 2801 0000 4bf3 5807 0000  IS-CGr(...K.X...
+00001160: 0048 4953 2d4e 4431 7229 0100 004b f458  .HIS-ND1r)...K.X
+00001170: 0700 0000 4849 532d 4344 3272 2a01 0000  ....HIS-CD2r*...
+00001180: 4bf5 5807 0000 0048 4953 2d43 4531 722b  K.X....HIS-CE1r+
+00001190: 0100 004b f658 0700 0000 4849 532d 4e45  ...K.X....HIS-NE
+000011a0: 3272 2c01 0000 4bf7 5805 0000 0048 4953  2r,...K.X....HIS
+000011b0: 2d48 722d 0100 004b f858 0600 0000 4849  -Hr-...K.X....HI
+000011c0: 532d 4841 722e 0100 004b f958 0700 0000  S-HAr....K.X....
+000011d0: 4849 532d 4842 3272 2f01 0000 4bfa 5807  HIS-HB2r/...K.X.
+000011e0: 0000 0048 4953 2d48 4233 7230 0100 004b  ...HIS-HB3r0...K
+000011f0: fb58 0700 0000 4849 532d 4844 3172 3101  .X....HIS-HD1r1.
+00001200: 0000 4bfc 5807 0000 0048 4953 2d48 4432  ..K.X....HIS-HD2
+00001210: 7232 0100 004b fd58 0700 0000 4849 532d  r2...K.X....HIS-
+00001220: 4845 3172 3301 0000 4bfe 5807 0000 0048  HE1r3...K.X....H
+00001230: 4953 2d48 4532 7234 0100 004b ff58 0500  IS-HE2r4...K.X..
+00001240: 0000 5345 522d 4e72 3501 0000 4d00 0158  ..SER-Nr5...M..X
+00001250: 0600 0000 5345 522d 4341 7236 0100 004d  ....SER-CAr6...M
+00001260: 0101 5805 0000 0053 4552 2d43 7237 0100  ..X....SER-Cr7..
+00001270: 004d 0201 5805 0000 0053 4552 2d4f 7238  .M..X....SER-Or8
+00001280: 0100 004d 0301 5806 0000 0053 4552 2d43  ...M..X....SER-C
+00001290: 4272 3901 0000 4d04 0158 0600 0000 5345  Br9...M..X....SE
+000012a0: 522d 4f47 723a 0100 004d 0501 5805 0000  R-OGr:...M..X...
+000012b0: 0053 4552 2d48 723b 0100 004d 0601 5806  .SER-Hr;...M..X.
+000012c0: 0000 0053 4552 2d48 4172 3c01 0000 4d07  ...SER-HAr<...M.
+000012d0: 0158 0700 0000 5345 522d 4842 3272 3d01  .X....SER-HB2r=.
+000012e0: 0000 4d08 0158 0700 0000 5345 522d 4842  ..M..X....SER-HB
+000012f0: 3372 3e01 0000 4d09 0158 0600 0000 5345  3r>...M..X....SE
+00001300: 522d 4847 723f 0100 004d 0a01 5805 0000  R-HGr?...M..X...
+00001310: 0054 4852 2d4e 7240 0100 004d 0b01 5806  .THR-Nr@...M..X.
+00001320: 0000 0054 4852 2d43 4172 4101 0000 4d0c  ...THR-CArA...M.
+00001330: 0158 0500 0000 5448 522d 4372 4201 0000  .X....THR-CrB...
+00001340: 4d0d 0158 0500 0000 5448 522d 4f72 4301  M..X....THR-OrC.
+00001350: 0000 4d0e 0158 0600 0000 5448 522d 4342  ..M..X....THR-CB
+00001360: 7244 0100 004d 0f01 5807 0000 0054 4852  rD...M..X....THR
+00001370: 2d4f 4731 7245 0100 004d 1001 5807 0000  -OG1rE...M..X...
+00001380: 0054 4852 2d43 4732 7246 0100 004d 1101  .THR-CG2rF...M..
+00001390: 5805 0000 0054 4852 2d48 7247 0100 004d  X....THR-HrG...M
+000013a0: 1201 5806 0000 0054 4852 2d48 4172 4801  ..X....THR-HArH.
+000013b0: 0000 4d13 0158 0600 0000 5448 522d 4842  ..M..X....THR-HB
+000013c0: 7249 0100 004d 1401 5807 0000 0054 4852  rI...M..X....THR
+000013d0: 2d48 4731 724a 0100 004d 1501 5808 0000  -HG1rJ...M..X...
+000013e0: 0054 4852 2d48 4732 3172 4b01 0000 4d16  .THR-HG21rK...M.
+000013f0: 0158 0800 0000 5448 522d 4847 3232 724c  .X....THR-HG22rL
+00001400: 0100 004d 1701 5808 0000 0054 4852 2d48  ...M..X....THR-H
+00001410: 4732 3372 4d01 0000 4d18 0158 0500 0000  G23rM...M..X....
+00001420: 4153 4e2d 4e72 4e01 0000 4d19 0158 0600  ASN-NrN...M..X..
+00001430: 0000 4153 4e2d 4341 724f 0100 004d 1a01  ..ASN-CArO...M..
+00001440: 5805 0000 0041 534e 2d43 7250 0100 004d  X....ASN-CrP...M
+00001450: 1b01 5805 0000 0041 534e 2d4f 7251 0100  ..X....ASN-OrQ..
+00001460: 004d 1c01 5806 0000 0041 534e 2d43 4272  .M..X....ASN-CBr
+00001470: 5201 0000 4d1d 0158 0600 0000 4153 4e2d  R...M..X....ASN-
+00001480: 4347 7253 0100 004d 1e01 5807 0000 0041  CGrS...M..X....A
+00001490: 534e 2d4f 4431 7254 0100 004d 1f01 5807  SN-OD1rT...M..X.
+000014a0: 0000 0041 534e 2d4e 4432 7255 0100 004d  ...ASN-ND2rU...M
+000014b0: 2001 5805 0000 0041 534e 2d48 7256 0100   .X....ASN-HrV..
+000014c0: 004d 2101 5806 0000 0041 534e 2d48 4172  .M!.X....ASN-HAr
+000014d0: 5701 0000 4d22 0158 0700 0000 4153 4e2d  W...M".X....ASN-
+000014e0: 4842 3272 5801 0000 4d23 0158 0700 0000  HB2rX...M#.X....
+000014f0: 4153 4e2d 4842 3372 5901 0000 4d24 0158  ASN-HB3rY...M$.X
+00001500: 0800 0000 4153 4e2d 4844 3231 725a 0100  ....ASN-HD21rZ..
+00001510: 004d 2501 5808 0000 0041 534e 2d48 4432  .M%.X....ASN-HD2
+00001520: 3272 5b01 0000 4d26 0158 0700 0000 414c  2r[...M&.X....AL
+00001530: 412d 4f58 5472 5c01 0000 4d27 0158 0600  A-OXTr\...M'.X..
+00001540: 0000 414c 412d 4832 725d 0100 004d 2801  ..ALA-H2r]...M(.
+00001550: 5806 0000 0041 4c41 2d48 3372 5e01 0000  X....ALA-H3r^...
+00001560: 4d29 0158 0700 0000 474c 552d 4845 3272  M).X....GLU-HE2r
+00001570: 5f01 0000 4d2a 0158 0700 0000 4153 502d  _...M*.X....ASP-
+00001580: 4844 3272 6001 0000 4d2b 0158 0500 0000  HD2r`...M+.X....
+00001590: 4d45 542d 4e72 6101 0000 4d2c 0158 0600  MET-Nra...M,.X..
+000015a0: 0000 4d45 542d 4341 7262 0100 004d 2d01  ..MET-CArb...M-.
+000015b0: 5805 0000 004d 4554 2d43 7263 0100 004d  X....MET-Crc...M
+000015c0: 2e01 5805 0000 004d 4554 2d4f 7264 0100  ..X....MET-Ord..
+000015d0: 004d 2f01 5806 0000 004d 4554 2d43 4272  .M/.X....MET-CBr
+000015e0: 6501 0000 4d30 0158 0600 0000 4d45 542d  e...M0.X....MET-
+000015f0: 4347 7266 0100 004d 3101 5806 0000 004d  CGrf...M1.X....M
+00001600: 4554 2d53 4472 6701 0000 4d32 0158 0600  ET-SDrg...M2.X..
+00001610: 0000 4d45 542d 4345 7268 0100 004d 3301  ..MET-CErh...M3.
+00001620: 5805 0000 004d 4554 2d48 7269 0100 004d  X....MET-Hri...M
+00001630: 3401 5806 0000 004d 4554 2d48 4172 6a01  4.X....MET-HArj.
+00001640: 0000 4d35 0158 0700 0000 4d45 542d 4842  ..M5.X....MET-HB
+00001650: 3272 6b01 0000 4d36 0158 0700 0000 4d45  2rk...M6.X....ME
+00001660: 542d 4842 3372 6c01 0000 4d37 0158 0700  T-HB3rl...M7.X..
+00001670: 0000 4d45 542d 4847 3272 6d01 0000 4d38  ..MET-HG2rm...M8
+00001680: 0158 0700 0000 4d45 542d 4847 3372 6e01  .X....MET-HG3rn.
+00001690: 0000 4d39 0158 0700 0000 4d45 542d 4845  ..M9.X....MET-HE
+000016a0: 3172 6f01 0000 4d3a 0158 0700 0000 4d45  1ro...M:.X....ME
+000016b0: 542d 4845 3272 7001 0000 4d3b 0158 0700  T-HE2rp...M;.X..
+000016c0: 0000 4d45 542d 4845 3372 7101 0000 4d3c  ..MET-HE3rq...M<
+000016d0: 0158 0500 0000 5452 502d 4e72 7201 0000  .X....TRP-Nrr...
+000016e0: 4d3d 0158 0600 0000 5452 502d 4341 7273  M=.X....TRP-CArs
+000016f0: 0100 004d 3e01 5805 0000 0054 5250 2d43  ...M>.X....TRP-C
+00001700: 7274 0100 004d 3f01 5805 0000 0054 5250  rt...M?.X....TRP
+00001710: 2d4f 7275 0100 004d 4001 5806 0000 0054  -Oru...M@.X....T
+00001720: 5250 2d43 4272 7601 0000 4d41 0158 0600  RP-CBrv...MA.X..
+00001730: 0000 5452 502d 4347 7277 0100 004d 4201  ..TRP-CGrw...MB.
+00001740: 5807 0000 0054 5250 2d43 4431 7278 0100  X....TRP-CD1rx..
+00001750: 004d 4301 5807 0000 0054 5250 2d43 4432  .MC.X....TRP-CD2
+00001760: 7279 0100 004d 4401 5807 0000 0054 5250  ry...MD.X....TRP
+00001770: 2d4e 4531 727a 0100 004d 4501 5807 0000  -NE1rz...ME.X...
+00001780: 0054 5250 2d43 4532 727b 0100 004d 4601  .TRP-CE2r{...MF.
+00001790: 5807 0000 0054 5250 2d43 4533 727c 0100  X....TRP-CE3r|..
+000017a0: 004d 4701 5807 0000 0054 5250 2d43 5a32  .MG.X....TRP-CZ2
+000017b0: 727d 0100 004d 4801 5807 0000 0054 5250  r}...MH.X....TRP
+000017c0: 2d43 5a33 727e 0100 004d 4901 5807 0000  -CZ3r~...MI.X...
+000017d0: 0054 5250 2d43 4832 727f 0100 004d 4a01  .TRP-CH2r....MJ.
+000017e0: 5805 0000 0054 5250 2d48 7280 0100 004d  X....TRP-Hr....M
+000017f0: 4b01 5806 0000 0054 5250 2d48 4172 8101  K.X....TRP-HAr..
+00001800: 0000 4d4c 0158 0700 0000 5452 502d 4842  ..ML.X....TRP-HB
+00001810: 3272 8201 0000 4d4d 0158 0700 0000 5452  2r....MM.X....TR
+00001820: 502d 4842 3372 8301 0000 4d4e 0158 0700  P-HB3r....MN.X..
+00001830: 0000 5452 502d 4844 3172 8401 0000 4d4f  ..TRP-HD1r....MO
+00001840: 0158 0700 0000 5452 502d 4845 3172 8501  .X....TRP-HE1r..
+00001850: 0000 4d50 0158 0700 0000 5452 502d 4845  ..MP.X....TRP-HE
+00001860: 3372 8601 0000 4d51 0158 0700 0000 5452  3r....MQ.X....TR
+00001870: 502d 485a 3272 8701 0000 4d52 0158 0700  P-HZ2r....MR.X..
+00001880: 0000 5452 502d 485a 3372 8801 0000 4d53  ..TRP-HZ3r....MS
+00001890: 0158 0700 0000 5452 502d 4848 3272 8901  .X....TRP-HH2r..
+000018a0: 0000 4d54 0158 0700 0000 474c 592d 4f58  ..MT.X....GLY-OX
+000018b0: 5472 8a01 0000 4d55 0158 0600 0000 5052  Tr....MU.X....PR
+000018c0: 4f2d 4832 728b 0100 004d 5601 5807 0000  O-H2r....MV.X...
+000018d0: 0050 4845 2d4f 5854 728c 0100 004d 5701  .PHE-OXTr....MW.
+000018e0: 5807 0000 0047 4c4e 2d4f 5854 728d 0100  X....GLN-OXTr...
+000018f0: 004d 5801 5806 0000 0053 4552 2d48 3272  .MX.X....SER-H2r
+00001900: 8e01 0000 4d59 0158 0600 0000 5345 522d  ....MY.X....SER-
+00001910: 4833 728f 0100 004d 5a01 5807 0000 0054  H3r....MZ.X....T
+00001920: 4852 2d4f 5854 7290 0100 004d 5b01 5807  HR-OXTr....M[.X.
+00001930: 0000 0047 4c55 2d4f 5854 7291 0100 004d  ...GLU-OXTr....M
+00001940: 5c01 5806 0000 0047 4c59 2d48 3272 9201  \.X....GLY-H2r..
+00001950: 0000 4d5d 0158 0600 0000 474c 592d 4833  ..M].X....GLY-H3
+00001960: 7293 0100 004d 5e01 5806 0000 004d 4554  r....M^.X....MET
+00001970: 2d48 3272 9401 0000 4d5f 0158 0600 0000  -H2r....M_.X....
+00001980: 4d45 542d 4833 7295 0100 004d 6001 5807  MET-H3r....M`.X.
+00001990: 0000 0048 4953 2d4f 5854 7296 0100 004d  ...HIS-OXTr....M
+000019a0: 6101 5807 0000 0049 4c45 2d4f 5854 7297  a.X....ILE-OXTr.
+000019b0: 0100 004d 6201 5806 0000 004c 5953 2d48  ...Mb.X....LYS-H
+000019c0: 3272 9801 0000 4d63 0158 0600 0000 4c59  2r....Mc.X....LY
+000019d0: 532d 4833 7299 0100 004d 6401 5806 0000  S-H3r....Md.X...
+000019e0: 0056 414c 2d48 3272 9a01 0000 4d65 0158  .VAL-H2r....Me.X
+000019f0: 0600 0000 5641 4c2d 4833 729b 0100 004d  ....VAL-H3r....M
+00001a00: 6601 5806 0000 0041 534e 2d48 3272 9c01  f.X....ASN-H2r..
+00001a10: 0000 4d67 0158 0600 0000 4153 4e2d 4833  ..Mg.X....ASN-H3
+00001a20: 729d 0100 004d 6801 5807 0000 0041 5247  r....Mh.X....ARG
+00001a30: 2d4f 5854 729e 0100 004d 6901 5807 0000  -OXTr....Mi.X...
+00001a40: 0041 534e 2d4f 5854 729f 0100 004d 6a01  .ASN-OXTr....Mj.
+00001a50: 5806 0000 0054 4852 2d48 3272 a001 0000  X....THR-H2r....
+00001a60: 4d6b 0158 0600 0000 5448 522d 4833 72a1  Mk.X....THR-H3r.
+00001a70: 0100 004d 6c01 5807 0000 0053 4552 2d4f  ...Ml.X....SER-O
+00001a80: 5854 72a2 0100 004d 6d01 5807 0000 0050  XTr....Mm.X....P
+00001a90: 524f 2d4f 5854 72a3 0100 004d 6e01 5806  RO-OXTr....Mn.X.
+00001aa0: 0000 0050 4845 2d48 3272 a401 0000 4d6f  ...PHE-H2r....Mo
+00001ab0: 0158 0600 0000 5048 452d 4833 72a5 0100  .X....PHE-H3r...
+00001ac0: 004d 7001 5807 0000 0053 4552 2d48 5854  .Mp.X....SER-HXT
+00001ad0: 72a6 0100 004d 7101 5806 0000 0041 5247  r....Mq.X....ARG
+00001ae0: 2d48 3272 a701 0000 4d72 0158 0600 0000  -H2r....Mr.X....
+00001af0: 4152 472d 4833 72a8 0100 004d 7301 5807  ARG-H3r....Ms.X.
+00001b00: 0000 004c 4555 2d4f 5854 72a9 0100 004d  ...LEU-OXTr....M
+00001b10: 7401 5806 0000 0049 4c45 2d48 3272 aa01  t.X....ILE-H2r..
+00001b20: 0000 4d75 0158 0600 0000 494c 452d 4833  ..Mu.X....ILE-H3
+00001b30: 72ab 0100 004d 7601 5806 0000 0047 4c4e  r....Mv.X....GLN
+00001b40: 2d48 3272 ac01 0000 4d77 0158 0600 0000  -H2r....Mw.X....
+00001b50: 474c 4e2d 4833 72ad 0100 004d 7801 5807  GLN-H3r....Mx.X.
+00001b60: 0000 004c 5953 2d4f 5854 72ae 0100 004d  ...LYS-OXTr....M
+00001b70: 7901 5806 0000 004c 4555 2d48 3272 af01  y.X....LEU-H2r..
+00001b80: 0000 4d7a 0158 0600 0000 4c45 552d 4833  ..Mz.X....LEU-H3
+00001b90: 72b0 0100 004d 7b01 5806 0000 0041 5350  r....M{.X....ASP
+00001ba0: 2d48 3272 b101 0000 4d7c 0158 0600 0000  -H2r....M|.X....
+00001bb0: 4153 502d 4833 72b2 0100 004d 7d01 5807  ASP-H3r....M}.X.
+00001bc0: 0000 0056 414c 2d4f 5854 72b3 0100 004d  ...VAL-OXTr....M
+00001bd0: 7e01 5807 0000 0054 5250 2d4f 5854 72b4  ~.X....TRP-OXTr.
+00001be0: 0100 004d 7f01 5806 0000 0047 4c55 2d48  ...M..X....GLU-H
+00001bf0: 3272 b501 0000 4d80 0158 0600 0000 474c  2r....M..X....GL
+00001c00: 552d 4833 72b6 0100 004d 8101 5807 0000  U-H3r....M..X...
+00001c10: 0043 5953 2d4f 5854 72b7 0100 004d 8201  .CYS-OXTr....M..
+00001c20: 5807 0000 0041 5350 2d4f 5854 72b8 0100  X....ASP-OXTr...
+00001c30: 004d 8301 5807 0000 0054 5952 2d4f 5854  .M..X....TYR-OXT
+00001c40: 72b9 0100 004d 8401 5806 0000 0043 5953  r....M..X....CYS
+00001c50: 2d48 3272 ba01 0000 4d85 0158 0600 0000  -H2r....M..X....
+00001c60: 4359 532d 4833 72bb 0100 004d 8601 5806  CYS-H3r....M..X.
+00001c70: 0000 0054 5952 2d48 3272 bc01 0000 4d87  ...TYR-H2r....M.
+00001c80: 0158 0600 0000 5459 522d 4833 72bd 0100  .X....TYR-H3r...
+00001c90: 004d 8801 5806 0000 0054 5250 2d48 3272  .M..X....TRP-H2r
+00001ca0: be01 0000 4d89 0158 0600 0000 5452 502d  ....M..X....TRP-
+00001cb0: 4833 72bf 0100 004d 8a01 5807 0000 004d  H3r....M..X....M
+00001cc0: 4554 2d4f 5854 72c0 0100 004d 8b01 5806  ET-OXTr....M..X.
+00001cd0: 0000 0041 4c41 2d44 3172 c101 0000 4d8c  ...ALA-D1r....M.
+00001ce0: 0158 0700 0000 5452 502d 4445 3172 c201  .X....TRP-DE1r..
+00001cf0: 0000 4d8d 0158 0600 0000 5459 522d 4448  ..M..X....TYR-DH
+00001d00: 72c3 0100 004d 8e01 5808 0000 0041 534e  r....M..X....ASN
+00001d10: 2d44 4432 3172 c401 0000 4d8f 0158 0600  -DD21r....M..X..
+00001d20: 0000 5345 522d 4447 72c5 0100 004d 9001  ..SER-DGr....M..
+00001d30: 5807 0000 0054 4852 2d44 4731 72c6 0100  X....THR-DG1r...
+00001d40: 004d 9101 5807 0000 004c 5953 2d44 5a31  .M..X....LYS-DZ1
+00001d50: 72c7 0100 004d 9201 5806 0000 0048 4953  r....M..X....HIS
+00001d60: 2d48 3272 c801 0000 4d93 0158 0600 0000  -H2r....M..X....
+00001d70: 4849 532d 4833 72c9 0100 004d 9401 5806  HIS-H3r....M..X.
+00001d80: 0000 0056 414c 2d44 3172 ca01 0000 4d95  ...VAL-D1r....M.
+00001d90: 0158 0500 0000 4c45 552d 4472 cb01 0000  .X....LEU-Dr....
+00001da0: 4d96 0158 0500 0000 5345 522d 4472 cc01  M..X....SER-Dr..
+00001db0: 0000 4d97 0158 0500 0000 474c 552d 4472  ..M..X....GLU-Dr
+00001dc0: cd01 0000 4d98 0158 0500 0000 5452 502d  ....M..X....TRP-
+00001dd0: 4472 ce01 0000 4d99 0158 0500 0000 474c  Dr....M..X....GL
+00001de0: 4e2d 4472 cf01 0000 4d9a 0158 0500 0000  N-Dr....M..X....
+00001df0: 414c 412d 4472 d001 0000 4d9b 0158 0500  ALA-Dr....M..X..
+00001e00: 0000 5641 4c2d 4472 d101 0000 4d9c 0158  ..VAL-Dr....M..X
+00001e10: 0500 0000 4153 502d 4472 d201 0000 4d9d  ....ASP-Dr....M.
+00001e20: 0158 0500 0000 474c 592d 4472 d301 0000  .X....GLY-Dr....
+00001e30: 4d9e 0158 0500 0000 5048 452d 4472 d401  M..X....PHE-Dr..
+00001e40: 0000 4d9f 0158 0500 0000 4c59 532d 4472  ..M..X....LYS-Dr
+00001e50: d501 0000 4da0 0158 0500 0000 4849 532d  ....M..X....HIS-
+00001e60: 4472 d601 0000 4da1 0158 0500 0000 4152  Dr....M..X....AR
+00001e70: 472d 4472 d701 0000 4da2 0158 0500 0000  G-Dr....M..X....
+00001e80: 5448 522d 4472 d801 0000 4da3 0158 0500  THR-Dr....M..X..
+00001e90: 0000 494c 452d 4472 d901 0000 4da4 0158  ..ILE-Dr....M..X
+00001ea0: 0700 0000 414c 412d 4858 5472 da01 0000  ....ALA-HXTr....
+00001eb0: 4da5 0158 0700 0000 4152 472d 4858 5472  M..X....ARG-HXTr
+00001ec0: db01 0000 4da6 0158 0500 0000 5459 522d  ....M..X....TYR-
+00001ed0: 4472 dc01 0000 4da7 0158 0700 0000 4c59  Dr....M..X....LY
+00001ee0: 532d 445a 3372 dd01 0000 4da8 0158 0700  S-DZ3r....M..X..
+00001ef0: 0000 4c59 532d 445a 3272 de01 0000 4da9  ..LYS-DZ2r....M.
+00001f00: 0158 0700 0000 4849 532d 4445 3272 df01  .X....HIS-DE2r..
+00001f10: 0000 4daa 0158 0700 0000 4849 532d 4444  ..M..X....HIS-DD
+00001f20: 3172 e001 0000 4dab 0158 0600 0000 4152  1r....M..X....AR
+00001f30: 472d 4445 72e1 0100 004d ac01 5805 0000  G-DEr....M..X...
+00001f40: 004d 4554 2d44 72e2 0100 004d ad01 5808  .MET-Dr....M..X.
+00001f50: 0000 0041 5247 2d44 4831 3172 e301 0000  ...ARG-DH11r....
+00001f60: 4dae 0158 0600 0000 414c 412d 4432 72e4  M..X....ALA-D2r.
+00001f70: 0100 004d af01 5805 0000 0044 4654 2d4f  ...M..X....DFT-O
+00001f80: 72e5 0100 004d b001 5805 0000 0044 4654  r....M..X....DFT
+00001f90: 2d43 72e6 0100 004d b101 5805 0000 0044  -Cr....M..X....D
+00001fa0: 4654 2d48 72e7 0100 004d b201 5805 0000  FT-Hr....M..X...
+00001fb0: 0044 4654 2d4e 72e8 0100 004d b301 5805  .DFT-Nr....M..X.
+00001fc0: 0000 0043 4153 2d43 72e9 0100 004d b401  ...CAS-Cr....M..
+00001fd0: 5805 0000 0043 4153 2d4f 72ea 0100 004d  X....CAS-Or....M
+00001fe0: b501 5805 0000 0043 4153 2d53 72eb 0100  ..X....CAS-Sr...
+00001ff0: 004d b601 5805 0000 0043 4153 2d46 72ec  .M..X....CAS-Fr.
+00002000: 0100 004d b701 5805 0000 0043 4153 2d48  ...M..X....CAS-H
+00002010: 72ed 0100 004d b801 5805 0000 0043 4153  r....M..X....CAS
+00002020: 2d4e 72ee 0100 004d b901 5806 0000 0043  -Nr....M..X....C
+00002030: 4153 2d43 6c72 ef01 0000 4dba 0158 0500  AS-Clr....M..X..
+00002040: 0000 4341 532d 5072 f001 0000 4dbb 0175  ..CAS-Pr....M..u
+00002050: 752e                                     u.
```

### Comparing `nmrgnn-data-0.7/nmrdata/data/standards.pb` & `nmrgnn-data-1.1.0/nmrdata/data/standards.pb`

 * *Files identical despite different names*

### Comparing `nmrgnn-data-0.7/nmrdata/loading.py` & `nmrgnn-data-1.1.0/nmrdata/loading.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,27 +12,28 @@
 def load_records(filename):
     data = tf.data.TFRecordDataset(
         filename, compression_type='GZIP').map(data_parse)
     return data.map(data_parse_dict)
 
 
 def data_parse_dict(*record):
-    atom_number, neighbor_number, bond_inputs, atom_inputs, peak_inputs, mask_inputs, name_inputs, class_input, record_index = record
+    atom_number, neighbor_number, bond_inputs, pos_inputs, atom_inputs, peak_inputs, mask_inputs, name_inputs, class_input, record_index = record
     return {'natoms': atom_number,
             'nneigh': neighbor_number,
             'features': atom_inputs,
             'nlist': bond_inputs,
+            'positions': pos_inputs,
             'peaks': peak_inputs,
             'mask': mask_inputs,
             'name': name_inputs,
             'class': class_input,
             'index': record_index}
 
 
-@tf.function(experimental_compile=True)
+@tf.function(experimental_relax_shapes=True)
 def nlist_model(positions, NN, sorted=False):
     M = tf.shape(input=positions)[0]
     # adjust NN
     NN = tf.minimum(NN, M)
     # Making 3 dim CG nlist
     qexpand = tf.expand_dims(positions, 1)  # one column
     qTexpand = tf.expand_dims(positions, 0)  # one row
@@ -92,41 +93,47 @@
 
 
 def data_parse(proto):
     features = {
         'atom-number': tf.io.FixedLenFeature([], tf.int64),
         'neighbor-number': tf.io.FixedLenFeature([], tf.int64),
         'bond-data': tf.io.VarLenFeature(tf.float32),
+        'position-data': tf.io.VarLenFeature(tf.float32),
         'atom-data': tf.io.VarLenFeature(tf.int64),
         'peak-data': tf.io.VarLenFeature(tf.float32),
         'mask-data': tf.io.VarLenFeature(tf.float32),
         'name-data': tf.io.VarLenFeature(tf.int64),
         'residue': tf.io.FixedLenFeature([1], tf.int64),
         'indices': tf.io.FixedLenFeature([3], tf.int64)
     }
     parsed_features = tf.io.parse_single_example(
         serialized=proto, features=features)
     # convert our features from sparse to dense
     atom_number = parsed_features['atom-number']
     neighbor_number = parsed_features['neighbor-number']
     bonds = tf.reshape(tf.sparse.to_dense(
         parsed_features['bond-data'], default_value=0), (atom_number, neighbor_number, 3))
-
+    if 'position-data' in parsed_features:
+        positions = tf.reshape(tf.sparse.to_dense(
+            parsed_features['position-data'], default_value=0), (atom_number, 3))
+    else:
+        positions = None
     atoms = tf.sparse.to_dense(
         parsed_features['atom-data'], default_value=0)
     peaks = tf.sparse.to_dense(
         parsed_features['peak-data'], default_value=0)
     mask = tf.sparse.to_dense(
         parsed_features['mask-data'], default_value=0)
     names = tf.sparse.to_dense(
         parsed_features['name-data'], default_value=0)
 
     return (parsed_features['atom-number'],
             parsed_features['neighbor-number'],
             bonds,
+            positions,
             atoms,
             peaks,
             mask,
             names,
             parsed_features['residue'],
             parsed_features['indices'])
 
@@ -143,66 +150,71 @@
 
 
 def data_shorten(*args, embeddings, label_info=False):
     embeddings = load_embeddings(embeddings)
     N = args[0]
     NN = args[1]
     nlist_full = args[2]
-    nodes = args[3]
-    labels = args[4]
-    mask = args[5]
-    names = args[6]
+    pos = args[3]
+    nodes = args[4]
+    labels = args[5]
+    mask = args[6]
+    names = args[7]
     edges = nlist_full[:, :, 0]
     inv_degree = tf.squeeze(tf.math.divide_no_nan(1.,
                                                   tf.reduce_sum(tf.cast(nlist_full[:, :, 0] > 0, tf.float32), axis=1)))
     nlist = tf.cast(nlist_full[:, :, 1], tf.int32)
     nodes = tf.one_hot(nodes, len(embeddings['atom']))
 
     if label_info:
-        return (nodes, nlist, edges, inv_degree), tf.stack([labels, tf.cast(names, labels.dtype), mask], axis=1), mask
-    return (nodes, nlist, edges, inv_degree), labels, mask
+        return (nodes, nlist, edges, inv_degree), tf.stack([labels, tf.cast(names, labels.dtype), mask], axis=1), mask[:, None]
+    return (nodes, nlist, edges, inv_degree), labels, mask[:, None]
 
 
-def make_tfrecord(atom_data, mask_data, nlist, peak_data, residue, atom_names, weights=None, indices=np.zeros((3, 1), dtype=np.int64)):
+def make_tfrecord(atom_data, mask_data, nlist, pos, peak_data, residue, atom_names, weights=None, indices=np.zeros((3, 1), dtype=np.int64)):
     '''
     Write out the TF record.
 
       atom_data - N ints containing atom indixes
       mask_data - N floats containing 1/0 for which atoms are begin considered
       nlist     - N x M x 3 floats neighbor list:
                     :,:,0 -> distance
                     :,:,1 -> neighbor index
                     :,:,2 -> bond count/type
+      pos       - N x 3 array of positions
       peak_data - N containing peak data for training (0 for prediction)
       residue     - N ints indicating the residue of the atom (for validation)
       atom_names  - N ints indicating the name of the atom  (for validation)
       indices       - 3 ints indices to attach to record (for validation)
     '''
     features = {}
     # nlist
     N = atom_data.shape[0]
     NN = nlist.shape[1]
     assert mask_data.shape[0] == N
     assert nlist.shape[0] == N and nlist.shape[2] == 3
+    assert pos.shape[0] == N and pos.shape[1] == 3
     assert peak_data.shape[0] == N
     assert atom_names.shape[0] == N
     assert len(indices) == 3
     if np.any(np.isnan(peak_data)):
         raise ValueError('Found nan in your data!')
         # Use code below if you do not care about nans
         peak_data[np.isnan(peak_data)] = 0
         mask_data[np.isnan(peak_data)] = 0
     if np.any(np.abs(peak_data) > 10000):
-        raise ValueError('Found very large peaks, |v| > 10000')
+        raise ValueError('Found very large peaks, |v| > 10000', peak_data)
     features['atom-number'] = tf.train.Feature(
         int64_list=tf.train.Int64List(value=[N]))
     features['neighbor-number'] = tf.train.Feature(
         int64_list=tf.train.Int64List(value=[NN]))
     features['bond-data'] = tf.train.Feature(
         float_list=tf.train.FloatList(value=nlist.flatten()))
+    features['position-data'] = tf.train.Feature(
+        float_list=tf.train.FloatList(value=pos.flatten()))
     features['atom-data'] = tf.train.Feature(
         int64_list=tf.train.Int64List(value=atom_data.flatten()))
     features['peak-data'] = tf.train.Feature(
         float_list=tf.train.FloatList(value=peak_data.flatten()))
     features['mask-data'] = tf.train.Feature(
         float_list=tf.train.FloatList(value=mask_data.flatten()))
     features['name-data'] = tf.train.Feature(
```

### Comparing `nmrgnn-data-0.7/nmrdata/parse/add_dssp.py` & `nmrgnn-data-1.1.0/nmrdata/parse/add_dssp.py`

 * *Files identical despite different names*

### Comparing `nmrgnn-data-0.7/nmrdata/parse/add_weights.py` & `nmrgnn-data-1.1.0/nmrdata/parse/add_weights.py`

 * *Files identical despite different names*

### Comparing `nmrgnn-data-0.7/nmrdata/parse/label_standardize.py` & `nmrgnn-data-1.1.0/nmrdata/parse/label_standardize.py`

 * *Files identical despite different names*

### Comparing `nmrgnn-data-0.7/nmrdata/parse/main.py` & `nmrgnn-data-1.1.0/nmrdata/parse/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     raise ModuleNotFoundError(
         'To use parsing, you must install openmm and extra dependencies with pip install nmrdata[parse]')
 
 
 from .protein_tfrecords import parse_refdb
 from .shiftml_tfrecords import parse_shiftml
 from .metabolite_tfrecords import parse_metabolites
+from .cascade_tfrecords import parse_cascade
 
 
 @click.group()
 def nmrparse():
     pass
 
 
@@ -40,7 +41,8 @@
     PDBFile.writeFile(fixer.topology, fixer.positions, open(output_pdb, 'w'))
 
 
 nmrparse.add_command(parse_refdb)
 nmrparse.add_command(parse_metabolites)
 nmrparse.add_command(parse_shiftml)
 nmrparse.add_command(clean_pdb)
+nmrparse.add_command(parse_cascade)
```

### Comparing `nmrgnn-data-0.7/nmrdata/parse/metabolite_tfrecords.py` & `nmrgnn-data-1.1.0/nmrdata/parse/metabolite_tfrecords.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,25 +79,23 @@
         m.AddAtom(Chem.Atom(a))
     for i in range(len(atoms)):
         for j in range(i, len(atoms)):
             if A[i, j] > 0:
                 m.AddBond(i, j, bonds[A[i, j]])
     mol = m.GetMol()
     try:
-        AllChem.EmbedMolecule(mol)
-        # Not necessary according to current docs
-        '''
         mol.UpdatePropertyCache(strict=False)
-        for i in range(1000):
-            r = AllChem.MMFFOptimizeMolecule(mol, maxIters=100)
-            if r == 0:
-                break
-            if r == -1:
-                raise ValueError()
-        '''
+        AllChem.EmbedMolecule(mol)
+        # Not necessary according to current docs (?)
+        # for i in range(1000):
+        #    r = AllChem.MMFFOptimizeMolecule(mol, maxIters=100)
+        #    if r == 0:
+        #        break
+        #    if r == -1:
+        #        raise ValueError()
     except (ValueError, RuntimeError) as e:
         print('Unable to process')
         print(Chem.MolToSmiles(mol))
         raise e
     for c in mol.GetConformers():
         pos = c.GetPositions()
         N = len(pos)
@@ -137,18 +135,18 @@
         if False:
             # debugging
             print(nlist[:len(atoms)])
             a1, a2 = np.nonzero(A)
             for a1i, a2i in zip(a1, a2):
                 print(a1i, a2i)
             exit()
-        yield nlist
+        yield np_pos, nlist
 
 
-@click.command()
+@click.command('metabolites')
 @click.argument('data_dir')
 @click.argument('output_name')
 @click.option('--embeddings', default=None, help='path to custom embeddings file')
 @click.option('--neighbor-number', default=16, help='The model specific size of neighbor lists')
 def parse_metabolites(data_dir, output_name, embeddings, neighbor_number):
 
     embeddings = load_embeddings(embeddings)
@@ -168,17 +166,17 @@
             class_label = 'MB'
             if class_label not in embeddings['class']:
                 embeddings['class'][class_label] = len(embeddings['class'])
             peak_data = prepare_labels(rd)
             name_data = names
             mask_data = (peak_data != 0) * 1.0
             try:
-                for ci, nlist in enumerate(adj_to_nlist(atoms, bond_data, embeddings, neighbor_number)):
+                for ci, (pos, nlist) in enumerate(adj_to_nlist(atoms, bond_data, embeddings, neighbor_number)):
                     pbar.set_description('{}:{}. Successes: {}'.format(
                         class_label, ci, successes))
                     record = make_tfrecord(
-                        atom_data, mask_data, nlist, peak_data, embeddings['class'][class_label], name_data)
+                        atom_data, mask_data, nlist, pos, peak_data, embeddings['class'][class_label], name_data)
                     writer.write(record.SerializeToString())
             except ValueError as e:
                 continue
             successes += 1
     save_embeddings(embeddings, 'new-embeddings.pb')
```

### Comparing `nmrgnn-data-0.7/nmrdata/parse/prepare_shiftx_records.py` & `nmrgnn-data-1.1.0/nmrdata/parse/prepare_shiftx_records.py`

 * *Files identical despite different names*

### Comparing `nmrgnn-data-0.7/nmrdata/parse/protein_tfrecords.py` & `nmrgnn-data-1.1.0/nmrdata/parse/protein_tfrecords.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,16 +49,14 @@
                 peaks[-1]['index'] = srid
     return peaks
 
 
 def process_corr(path, debug, shiftx_style):
 
     peaks = pyparse_corr(path, shiftx_style)
-    print(peaks)
-    exit()
 
     if len(peaks) == 0:
         raise ValueError('Could not parse file')
 
     sequence_map = {}
 
     # sequence map -> key is residue index, output is peak index
@@ -114,15 +112,14 @@
     return -offset[0], -offset[1]
 
 
 def process_pdb(path, corr_path, chain_id,
                 gsd_file, embedding_dicts, neighbor_number, neighbor_margin=8,
                 debug=False, units=unit.nanometer, frame_number=3, model_index=0,
                 log_file=None, shiftx_style=False):
-
     global MA_LOST_FRAGS
     if shiftx_style:
         frame_number = 1
     # load pdb
     pdb = app.PDBFile(path)
 
     # load cs sets
@@ -197,15 +194,15 @@
             pdb_offset, seq_offset = align(pdb_seq, peak_seq, debug)
             # TOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOODDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDOOOOOOOOOOOOOOOOOOOOOOO?????
             # Maybe it's ok
             pdb_offset = 0
             if debug:
                 print('pdb_offset', pdb_offset)
                 print('seq_offset', seq_offset)
-                #print(sequence_map)
+                # print(sequence_map)
                 # now check alignment - rarely perfect
                 saw_one = False
                 aligned = 0
                 for i in range(len(residues)):
                     segid = int(residues[i].id) + pdb_offset
                     saw_one = pdb_seq[segid] == residues[i].name
                     if not saw_one:
@@ -360,23 +357,23 @@
                 raise RuntimeError()
             continue
         if gsd_file is not None:
             snapshot = write_record_traj(positions, atoms, mask, nlist, peaks,
                                          embedding_dicts['class'][residues[ri].name], names, embedding_dicts)
             snapshot.configuration.step = len(gsd_file)
             gsd_file.append(snapshot)
-        result.append(make_tfrecord(atoms, mask, nlist, peaks, embedding_dicts['class'][residues[ri].name], names, indices=np.array(
+        result.append(make_tfrecord(atoms, mask, nlist, positions, peaks, embedding_dicts['class'][residues[ri].name], names, indices=np.array(
             [model_index, fi, int(residues[ri].id)], dtype=np.int64)))
         if log_file is not None:
             log_file.write('{} {} {} {} {} {} {} {}\n'.format(path.split('/')[-1], corr_path.split(
                 '/')[-1], chain_id, len(peak_successes), len(gsd_file), model_index, fi, residues[ri].id))
     return result, len(peak_successes) / len(peak_data), len(result), peak_count
 
 
-@click.command()
+@click.command('refdb')
 @click.argument('protein_dir')
 @click.argument('output_name')
 @click.option('--embeddings', default=None, help='path to custom embeddings file')
 @click.option('--shiftx/--no-shiftx', default=False, help='Are these the cleaned shiftx files?')
 @click.option('--debug/--no-debug', default=False)
 @click.option('--pdb_filter', default=None, help='file containing list of pdbs to exclude')
 @click.option('--invert_filter', default=False, help='Invert the pdb filter to only include the pdbs')
@@ -391,15 +388,15 @@
             pdb_filter_list = set([x.split()[0] for x in f.readlines()])
         print('Will filter pdbs from', pdb_filter, flush=True)
 
     # load embedding information
     embedding_dicts = load_embeddings(embeddings)
 
     # load data info
-    with open(os.path.join(protein_dir,'data.pb'), 'rb') as f:
+    with open(os.path.join(protein_dir, 'data.pb'), 'rb') as f:
         protein_data = pickle.load(f)
 
     items = list(protein_data.values())
     records = 0
     peaks = 0
     # turn off GPU for more memory if desired
     # config.graph_options.optimizer_options.global_jit_level = tf.OptimizerOptions.ON_1
@@ -414,22 +411,22 @@
             if invert_filter:
                 if pdb_filter_list is not None and entry['pdb_id'] not in pdb_filter_list:
                     continue
             else:
                 if pdb_filter_list is not None and entry['pdb_id'] in pdb_filter_list:
                     continue
             try:
-                result, p, n, pc = process_pdb(os.path.join(protein_dir,entry['pdb_file']), os.path.join(protein_dir,entry['corr']), entry['chain'],
+                result, p, n, pc = process_pdb(os.path.join(protein_dir, entry['pdb_file']), os.path.join(protein_dir, entry['corr']), entry['chain'],
                                                gsd_file=gsd_file, debug=debug,
                                                embedding_dicts=embedding_dicts, neighbor_number=neighbor_number,
                                                model_index=index, log_file=rinfo, shiftx_style=shiftx)
                 pbar.set_description('Processed PDB {} ({}). Successes {} ({:.2}). Total Records: {}, Peaks: {}. Wrote frags: {}. Lost frags {}({})'.format(
                     entry['pdb_id'], entry['corr'], n, p, records, peaks, index % gsd_frag_period == 0, MA_LOST_FRAGS, MA_LOST_FRAGS / (MA_LOST_FRAGS + n + 1)))
                 # turned off for now
-                if False and len(result) == 0:
+                if False or len(result) == 0:
                     raise ValueError(
                         'Failed to find any records in' + entry['pdb_id'], entry['corr'])
                 for r in result:
                     writer.write(r.SerializeToString())
                 records += n
                 peaks += pc
                 rinfo.flush()
```

### Comparing `nmrgnn-data-0.7/nmrdata/parse/shiftml_tfrecords.py` & `nmrgnn-data-1.1.0/nmrdata/parse/shiftml_tfrecords.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import tensorflow as tf
 import numpy as np
 import pickle
 import io
 import tqdm
 from nmrdata import *
 
+
 def make_nlist(pos, embeddings, neighbor_number):
     # all nlists are non-bonded here
     N = pos.shape[0]
     pos_nlist = nlist_model(pos, neighbor_number)
-    nlist = np.zeros( (N, neighbor_number, 3) , dtype=np.float32)
+    nlist = np.zeros((N, neighbor_number, 3), dtype=np.float32)
     # a 0 -> non-bonded
     for index in range(N):
         for ni in range(len(pos_nlist[index])):
-            if pos_nlist[index, ni, 0] >= 100: # this is a large distance sentinel indicating not part of nlist
+            # this is a large distance sentinel indicating not part of nlist
+            if pos_nlist[index, ni, 0] >= 100:
                 continue
             j = int(pos_nlist[index, ni, 1])
             # / 10 to get to nm
             nlist[index, ni, 0] = pos_nlist[index, ni, 0] / 10
             nlist[index, ni, 1] = j
-            nlist[index,ni,2] = embeddings['nlist']['nonbonded']
+            nlist[index, ni, 2] = embeddings['nlist']['nonbonded']
         # pad out the nlist
         for index in range(N, N):
             for ni in range(neighbor_number):
                 nlist[index, ni, 0] = 0
                 nlist[index, ni, 1] = 0
                 nlist[index, ni, 2] = embeddings['nlist']['none']
     return nlist
@@ -35,15 +37,15 @@
         if not line:
             break
         N = int(line)
         name = ifile.readline().split('NAME=')[1]
         features = np.empty((N), dtype=np.int64)
         atom_names = np.empty((N), dtype=np.int64)
         pos = np.empty((N, 3), dtype=np.float32)
-        peaks = np.empty((N), dtype=np.float32)
+        peaks = np.zeros((N), dtype=np.float32)
         for i in range(N):
             sline = ifile.readline().split()
             e = sline[0]
             if e not in embeddings['atom']:
                 embeddings['atom'][e] = len(embeddings['atom'])
             features[i] = embeddings['atom'][e]
             atom_name = 'DFT-' + e
@@ -51,33 +53,35 @@
                 print('*******Adding new atom name*********')
                 embeddings['name'][atom_name] = len(embeddings['name'])
             atom_names[i] = embeddings['name'][atom_name]
             pos[i, :] = [float(s) for s in sline[1:4]]
             peaks[i] = float(sline[4])
         yield features, atom_names, pos, peaks
 
-@click.command()
+
+@click.command('shiftml')
 @click.argument('xyz_file')
 @click.argument('output_name')
 @click.option('--embeddings', default=None, help='path to custom embeddings file')
 @click.option('--neighbor-number', default=16, help='The model specific size of neighbor lists')
 def parse_shiftml(xyz_file, output_name, embeddings, neighbor_number):
 
     embeddings = load_embeddings(embeddings)
     with tf.io.TFRecordWriter(f'shiftml-{output_name}.tfrecord',
-                                     options=tf.io.TFRecordOptions(compression_type='GZIP')) as writer,\
-        open(xyz_file) as f:
+                              options=tf.io.TFRecordOptions(compression_type='GZIP')) as writer,\
+            open(xyz_file) as f:
         successes = 0
         pbar = tqdm.tqdm(parse_xyz(f, embeddings))
         for rd in pbar:
             atom_data, name_data, pos, peaks = rd
             class_label = 'DFT'
             if class_label not in embeddings['class']:
                 embeddings['class'][class_label] = len(embeddings['class'])
             mask_data = np.ones_like(atom_data).astype(np.float32)
             nlist = make_nlist(pos, embeddings, neighbor_number)
-            pbar.set_description('DFT with {} atoms. Successes: {}'.format(len(atom_data), successes))
-            record = make_tfrecord(atom_data, mask_data, nlist, peaks, embeddings['class'][class_label], name_data)
+            pbar.set_description(
+                'DFT with {} atoms. Successes: {}'.format(len(atom_data), successes))
+            record = make_tfrecord(
+                atom_data, mask_data, nlist, pos, peaks, embeddings['class'][class_label], name_data)
             writer.write(record.SerializeToString())
             successes += 1
     save_embeddings(embeddings, 'final-embeddings.pb')
-
```

### Comparing `nmrgnn-data-0.7/nmrdata/validation.py` & `nmrgnn-data-1.1.0/nmrdata/validation.py`

 * *Files 4% similar despite different names*

```diff
@@ -193,19 +193,19 @@
 
     # Now write out data
     with open(output, 'w') as f:
         for d in data:
             mask, peaks, name, index = [
                 d['mask'], d['peaks'], d['name'], d['index']]
             indices = np.nonzero(mask)
-            for b, i in zip(indices[0], indices[1]):
-                p = rinfo[index[b, 0].numpy()]
-                n = namedict[name[b, i].numpy()]
+            for i in indices[0]:
+                p = rinfo[index[0].numpy()]
+                n = namedict[name[i].numpy()]
                 f.write(
-                    ' '.join([p, str(index[b, 2].numpy()), *n.split('-'), str(peaks[b, i].numpy()), '\n']))
+                    ' '.join([p, str(index[2].numpy()), *n.split('-'), str(peaks[i].numpy()), '\n']))
     return
 
 
 @click.command()
 @click.argument('tfrecords')
 @click.argument('name_i')
 @click.argument('name_j')
```

### Comparing `nmrgnn-data-0.7/nmrgnn_data.egg-info/SOURCES.txt` & `nmrgnn-data-1.1.0/nmrgnn_data.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 nmrdata/version.py
 nmrdata/data/__init__.py
 nmrdata/data/embeddings.pb
 nmrdata/data/standards.pb
 nmrdata/parse/__init__.py
 nmrdata/parse/add_dssp.py
 nmrdata/parse/add_weights.py
+nmrdata/parse/cascade_tfrecords.py
 nmrdata/parse/label_standardize.py
 nmrdata/parse/main.py
 nmrdata/parse/metabolite_tfrecords.py
 nmrdata/parse/prepare_shiftx_records.py
 nmrdata/parse/protein_tfrecords.py
 nmrdata/parse/shiftml_tfrecords.py
 nmrgnn_data.egg-info/PKG-INFO
```

### Comparing `nmrgnn-data-0.7/setup.py` & `nmrgnn-data-1.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,21 +13,21 @@
       description='Chemical shift prediction dataset',
       author='Ziyue Yang, Andrew White',
       author_email='andrew.white@rochester.edu',
       url='https://github.com/ur-whitelab/nmrdata',
       license='MIT',
       packages=['nmrdata', 'nmrdata.data', 'nmrdata.parse'],
       install_requires=[
-          'tensorflow >= 2.3',
+          'tensorflow >= 2.7',
           'click',
-          'numpy>=1.18.5',
+          'numpy',
           'MDAnalysis ~= 2.0',
           'importlib_resources'],
       extras_require={
-          'parse': ['pdbfixer', 'biopython', 'gsd']
+          'parse': ['pdbfixer', 'biopython', 'gsd', 'rdkit-pypi']
       },
       zip_safe=True,
       entry_points='''
         [console_scripts]
         nmrparse=nmrdata.parse.main:nmrparse
         nmrdata=nmrdata.main:nmrdata
             ''',
```

