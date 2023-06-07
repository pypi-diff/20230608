# Comparing `tmp/boxhed-2.0.4.tar.gz` & `tmp/boxhed-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boxhed-2.0.4.tar", last modified: Wed Jun  7 00:13:45 2023, max compression
+gzip compressed data, was "boxhed-2.0.6.tar", last modified: Wed Jun  7 22:57:09 2023, max compression
```

## Comparing `boxhed-2.0.4.tar` & `boxhed-2.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-07 00:13:45.258593 boxhed-2.0.4/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       29 2023-05-30 19:24:43.000000 boxhed-2.0.4/MANIFEST.in
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      980 2023-06-07 00:13:45.258593 boxhed-2.0.4/PKG-INFO
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      825 2023-05-30 19:24:43.000000 boxhed-2.0.4/README.md
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-07 00:13:45.258593 boxhed-2.0.4/boxhed/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-05-30 19:24:43.000000 boxhed-2.0.4/boxhed/__init__.py
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    18195 2023-06-07 00:02:32.000000 boxhed-2.0.4/boxhed/boxhed.py
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    14339 2023-05-30 19:24:43.000000 boxhed-2.0.4/boxhed/model_selection.py
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     4836 2023-05-30 19:24:43.000000 boxhed-2.0.4/boxhed/utils.py
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-07 00:13:45.258593 boxhed-2.0.4/boxhed.egg-info/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      980 2023-06-07 00:13:45.000000 boxhed-2.0.4/boxhed.egg-info/PKG-INFO
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      296 2023-06-07 00:13:45.000000 boxhed-2.0.4/boxhed.egg-info/SOURCES.txt
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)        1 2023-06-07 00:13:45.000000 boxhed-2.0.4/boxhed.egg-info/dependency_links.txt
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)        1 2023-06-07 00:13:45.000000 boxhed-2.0.4/boxhed.egg-info/not-zip-safe
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       70 2023-06-07 00:13:45.000000 boxhed-2.0.4/boxhed.egg-info/requires.txt
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)        7 2023-06-07 00:13:45.000000 boxhed-2.0.4/boxhed.egg-info/top_level.txt
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       38 2023-06-07 00:13:45.258593 boxhed-2.0.4/setup.cfg
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      664 2023-06-07 00:11:22.000000 boxhed-2.0.4/setup.py
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-07 22:57:09.263919 boxhed-2.0.6/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       29 2023-06-07 00:34:05.000000 boxhed-2.0.6/MANIFEST.in
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      980 2023-06-07 22:57:09.263919 boxhed-2.0.6/PKG-INFO
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      825 2023-06-07 00:34:05.000000 boxhed-2.0.6/README.md
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-07 22:57:09.259920 boxhed-2.0.6/boxhed/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-07 00:34:05.000000 boxhed-2.0.6/boxhed/__init__.py
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    18195 2023-06-07 20:40:39.000000 boxhed-2.0.6/boxhed/boxhed.py
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    14495 2023-06-07 22:50:17.000000 boxhed-2.0.6/boxhed/model_selection.py
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     4836 2023-06-07 00:34:05.000000 boxhed-2.0.6/boxhed/utils.py
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-07 22:57:09.263919 boxhed-2.0.6/boxhed.egg-info/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      980 2023-06-07 22:57:09.000000 boxhed-2.0.6/boxhed.egg-info/PKG-INFO
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      296 2023-06-07 22:57:09.000000 boxhed-2.0.6/boxhed.egg-info/SOURCES.txt
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)        1 2023-06-07 22:57:09.000000 boxhed-2.0.6/boxhed.egg-info/dependency_links.txt
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)        1 2023-06-07 22:57:09.000000 boxhed-2.0.6/boxhed.egg-info/not-zip-safe
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       70 2023-06-07 22:57:09.000000 boxhed-2.0.6/boxhed.egg-info/requires.txt
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)        7 2023-06-07 22:57:09.000000 boxhed-2.0.6/boxhed.egg-info/top_level.txt
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       38 2023-06-07 22:57:09.263919 boxhed-2.0.6/setup.cfg
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      664 2023-06-07 22:50:47.000000 boxhed-2.0.6/setup.py
```

### Comparing `boxhed-2.0.4/PKG-INFO` & `boxhed-2.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boxhed
-Version: 2.0.4
+Version: 2.0.6
 Summary: BoXHED2.0
 Author: Arash Pakbin
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 **B**oosted e**X**act **H**azard **E**stimator with **D**ynamic covariates v2.0 (BoXHED2.0, pronounced 'box-head') is a software package for nonparametrically estimating hazard functions via gradient boosted trees. BoXHED2.0 accommodates both time-static and time-dependent covariates.
```

### Comparing `boxhed-2.0.4/README.md` & `boxhed-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `boxhed-2.0.4/boxhed/boxhed.py` & `boxhed-2.0.6/boxhed/boxhed.py`

 * *Files identical despite different names*

### Comparing `boxhed-2.0.4/boxhed/model_selection.py` & `boxhed-2.0.6/boxhed/model_selection.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,16 +225,14 @@
 
                 p = mp.Process(target = _run_batch_process, args = (param_dict_mngd, rslt_mngd))
 
                 p.start() 
                 p.join()
                 
                 p.terminate()
-                if p.exitcode != 0:
-                    raise MemoryError("ERROR: Cross validation did not finish successfully due to memory error. Consider reducing nthread and/or models_per_gpu to cut down on the memory used by cross validation.")
             
             smm.shutdown()
             
             self.rslts = list(rslt_mngd)
 
     def _calculate_output_statistics(self):
         def sort_pred(dict_):
@@ -248,14 +246,17 @@
                 sorted(zip(self.rslts,self.param_dicts_test), 
                 key=lambda pair: sort_pred(pair[1]))
                     ]
         srtd_rslts, srtd_param_dict_test = zip(*rslt__param_dict_test)
         srtd_rslts = np.array(srtd_rslts)
         srtd_rslts = srtd_rslts.reshape(-1, len(self.cv))
 
+        if 0 in srtd_rslts:
+            raise MemoryError("ERROR: Cross validation did not finish successfully due to memory error. Consider reducing nthread and/or models_per_gpu to cut down on the memory used by cross validation.")
+
         self.srtd_param_dict_test_scores = srtd_rslts.mean(axis=1)
         self.srtd_param_dict_test_std    = srtd_rslts.std(axis=1)
  
         self.srtd_param_dict_test = srtd_param_dict_test[0::len(self.cv)]
         for srtd_param_dict_test in self.srtd_param_dict_test:
             srtd_param_dict_test.pop('fold')
 
@@ -286,20 +287,28 @@
     ID_counts = [len(ID_unique_srtd)//num_folds] * num_folds
     for i in range(len(ID_unique_srtd)%num_folds):
         ID_counts[i]+=1
 
     assert sum(ID_counts)==len(ID_unique_srtd)
 
     fold_idxs = np.hstack([[i]*id_count for i, id_count in enumerate(ID_counts)])
-
+    '''
     if seed is not None:
         with temp_seed(seed):
             np.random.shuffle(fold_idxs)
     else:
         np.random.shuffle(fold_idxs)
+    '''
+    if seed is not None:
+        rng = np.random.default_rng(seed)
+        rng.shuffle(fold_idxs)
+        
+    else:
+        np.random.shuffle(fold_idxs) 
+
 
     gkf = []
     for fold_idx in range(num_folds):
         train_ids = ID_unique_srtd[np.where(fold_idxs!=fold_idx)[0]]
         test_ids  = ID_unique_srtd[np.where(fold_idxs==fold_idx)[0]]
         gkf.append((np.where(np.isin(ID, train_ids))[0], np.where(np.isin(ID, test_ids))[0]))
```

### Comparing `boxhed-2.0.4/boxhed/utils.py` & `boxhed-2.0.6/boxhed/utils.py`

 * *Files identical despite different names*

### Comparing `boxhed-2.0.4/boxhed.egg-info/PKG-INFO` & `boxhed-2.0.6/boxhed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boxhed
-Version: 2.0.4
+Version: 2.0.6
 Summary: BoXHED2.0
 Author: Arash Pakbin
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 **B**oosted e**X**act **H**azard **E**stimator with **D**ynamic covariates v2.0 (BoXHED2.0, pronounced 'box-head') is a software package for nonparametrically estimating hazard functions via gradient boosted trees. BoXHED2.0 accommodates both time-static and time-dependent covariates.
```

### Comparing `boxhed-2.0.4/setup.py` & `boxhed-2.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="boxhed",
-    version="2.0.4",
+    version="2.0.6",
     long_description=long_description,
     long_description_content_type='text/markdown',
     description="BoXHED2.0",
     author='Arash Pakbin',
     packages=find_packages(),
     python_requires=">=3.8",
     include_package_data=True,
```

