# Comparing `tmp/sgdml-1.0.0.tar.gz` & `tmp/sgdml-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sgdml-1.0.0.tar", last modified: Mon Jan  2 16:13:16 2023, max compression
+gzip compressed data, was "sgdml-1.0.1.tar", last modified: Thu Jun  8 12:53:02 2023, max compression
```

## Comparing `sgdml-1.0.0.tar` & `sgdml-1.0.1.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 stefan     (501) staff       (20)        0 2023-01-02 16:13:16.824263 sgdml-1.0.0/
--rw-r--r--   0 stefan     (501) staff       (20)     5594 2023-01-02 16:13:16.824393 sgdml-1.0.0/PKG-INFO
--rw-r--r--   0 stefan     (501) staff       (20)     3632 2023-01-02 16:10:51.000000 sgdml-1.0.0/README.md
--rw-r--r--   0 stefan     (501) staff       (20)       91 2023-01-02 16:10:51.000000 sgdml-1.0.0/pyproject.toml
-drwxr-xr-x   0 stefan     (501) staff       (20)        0 2023-01-02 16:13:16.820754 sgdml-1.0.0/scripts/
--rwxr-xr-x   0 stefan     (501) staff       (20)     5518 2023-01-02 16:10:51.000000 sgdml-1.0.0/scripts/sgdml_dataset_from_aims.py
--rwxr-xr-x   0 stefan     (501) staff       (20)     6762 2023-01-02 16:10:51.000000 sgdml-1.0.0/scripts/sgdml_dataset_from_extxyz.py
--rwxr-xr-x   0 stefan     (501) staff       (20)     5828 2023-01-02 16:10:51.000000 sgdml-1.0.0/scripts/sgdml_dataset_from_ipi.py
--rwxr-xr-x   0 stefan     (501) staff       (20)     2950 2023-01-02 16:10:51.000000 sgdml-1.0.0/scripts/sgdml_dataset_to_extxyz.py
--rwxr-xr-x   0 stefan     (501) staff       (20)     6055 2023-01-02 16:10:51.000000 sgdml-1.0.0/scripts/sgdml_dataset_via_ase.py
--rwxr-xr-x   0 stefan     (501) staff       (20)     3388 2023-01-02 16:10:51.000000 sgdml-1.0.0/scripts/sgdml_datasets_from_model.py
--rw-r--r--   0 stefan     (501) staff       (20)      316 2023-01-02 16:13:16.825441 sgdml-1.0.0/setup.cfg
--rw-r--r--   0 stefan     (501) staff       (20)     2004 2023-01-02 16:10:51.000000 sgdml-1.0.0/setup.py
-drwxr-xr-x   0 stefan     (501) staff       (20)        0 2023-01-02 16:13:16.821729 sgdml-1.0.0/sgdml/
--rw-r--r--   0 stefan     (501) staff       (20)     3591 2023-01-02 16:11:56.000000 sgdml-1.0.0/sgdml/__init__.py
--rw-r--r--   0 stefan     (501) staff       (20)    74967 2023-01-02 16:10:51.000000 sgdml-1.0.0/sgdml/cli.py
--rwxr-xr-x   0 stefan     (501) staff       (20)     5223 2023-01-02 16:10:51.000000 sgdml-1.0.0/sgdml/get.py
-drwxr-xr-x   0 stefan     (501) staff       (20)        0 2023-01-02 16:13:16.823002 sgdml-1.0.0/sgdml/intf/
--rwxr-xr-x   0 stefan     (501) staff       (20)        0 2023-01-02 16:10:51.000000 sgdml-1.0.0/sgdml/intf/__init__.py
--rwxr-xr-x   0 stefan     (501) staff       (20)     4188 2023-01-02 16:10:51.000000 sgdml-1.0.0/sgdml/intf/ase_calc.py
--rw-r--r--   0 stefan     (501) staff       (20)    46891 2023-01-02 16:10:51.000000 sgdml-1.0.0/sgdml/predict.py
-drwxr-xr-x   0 stefan     (501) staff       (20)        0 2023-01-02 16:13:16.823397 sgdml-1.0.0/sgdml/solvers/
--rwxr-xr-x   0 stefan     (501) staff       (20)        0 2023-01-02 16:10:51.000000 sgdml-1.0.0/sgdml/solvers/__init__.py
--rwxr-xr-x   0 stefan     (501) staff       (20)     5423 2023-01-02 16:10:51.000000 sgdml-1.0.0/sgdml/solvers/analytic.py
--rw-r--r--   0 stefan     (501) staff       (20)    28082 2023-01-02 16:10:51.000000 sgdml-1.0.0/sgdml/solvers/iterative.py
--rw-r--r--   0 stefan     (501) staff       (20)    40509 2023-01-02 16:10:51.000000 sgdml-1.0.0/sgdml/torchtools.py
--rw-r--r--   0 stefan     (501) staff       (20)    60606 2023-01-02 16:10:51.000000 sgdml-1.0.0/sgdml/train.py
-drwxr-xr-x   0 stefan     (501) staff       (20)        0 2023-01-02 16:13:16.824136 sgdml-1.0.0/sgdml/utils/
--rwxr-xr-x   0 stefan     (501) staff       (20)        0 2023-01-02 16:10:51.000000 sgdml-1.0.0/sgdml/utils/__init__.py
--rw-r--r--   0 stefan     (501) staff       (20)    17343 2023-01-02 16:10:51.000000 sgdml-1.0.0/sgdml/utils/desc.py
--rwxr-xr-x   0 stefan     (501) staff       (20)    19139 2023-01-02 16:10:51.000000 sgdml-1.0.0/sgdml/utils/io.py
--rwxr-xr-x   0 stefan     (501) staff       (20)    31377 2023-01-02 16:10:51.000000 sgdml-1.0.0/sgdml/utils/perm.py
--rwxr-xr-x   0 stefan     (501) staff       (20)    13361 2023-01-02 16:10:51.000000 sgdml-1.0.0/sgdml/utils/ui.py
-drwxr-xr-x   0 stefan     (501) staff       (20)        0 2023-01-02 16:13:16.822746 sgdml-1.0.0/sgdml.egg-info/
--rw-r--r--   0 stefan     (501) staff       (20)     5594 2023-01-02 16:13:16.000000 sgdml-1.0.0/sgdml.egg-info/PKG-INFO
--rw-r--r--   0 stefan     (501) staff       (20)      779 2023-01-02 16:13:16.000000 sgdml-1.0.0/sgdml.egg-info/SOURCES.txt
--rw-r--r--   0 stefan     (501) staff       (20)        1 2023-01-02 16:13:16.000000 sgdml-1.0.0/sgdml.egg-info/dependency_links.txt
--rw-r--r--   0 stefan     (501) staff       (20)       69 2023-01-02 16:13:16.000000 sgdml-1.0.0/sgdml.egg-info/entry_points.txt
--rw-r--r--   0 stefan     (501) staff       (20)        1 2023-01-02 16:13:16.000000 sgdml-1.0.0/sgdml.egg-info/not-zip-safe
--rw-r--r--   0 stefan     (501) staff       (20)       71 2023-01-02 16:13:16.000000 sgdml-1.0.0/sgdml.egg-info/requires.txt
--rw-r--r--   0 stefan     (501) staff       (20)        6 2023-01-02 16:13:16.000000 sgdml-1.0.0/sgdml.egg-info/top_level.txt
+drwxr-xr-x   0 stefan     (501) staff       (20)        0 2023-06-08 12:53:02.214548 sgdml-1.0.1/
+-rw-r--r--   0 stefan     (501) staff       (20)     1075 2023-06-08 12:49:26.000000 sgdml-1.0.1/LICENSE.txt
+-rw-r--r--   0 stefan     (501) staff       (20)     4567 2023-06-08 12:53:02.214610 sgdml-1.0.1/PKG-INFO
+-rw-r--r--   0 stefan     (501) staff       (20)     3649 2023-06-08 12:49:26.000000 sgdml-1.0.1/README.md
+-rw-r--r--   0 stefan     (501) staff       (20)       91 2023-06-08 12:49:26.000000 sgdml-1.0.1/pyproject.toml
+drwxr-xr-x   0 stefan     (501) staff       (20)        0 2023-06-08 12:53:02.211802 sgdml-1.0.1/scripts/
+-rwxr-xr-x   0 stefan     (501) staff       (20)     5518 2023-06-08 12:49:26.000000 sgdml-1.0.1/scripts/sgdml_dataset_from_aims.py
+-rwxr-xr-x   0 stefan     (501) staff       (20)     6762 2023-06-08 12:49:26.000000 sgdml-1.0.1/scripts/sgdml_dataset_from_extxyz.py
+-rwxr-xr-x   0 stefan     (501) staff       (20)     5828 2023-06-08 12:49:26.000000 sgdml-1.0.1/scripts/sgdml_dataset_from_ipi.py
+-rwxr-xr-x   0 stefan     (501) staff       (20)     2950 2023-06-08 12:49:26.000000 sgdml-1.0.1/scripts/sgdml_dataset_to_extxyz.py
+-rwxr-xr-x   0 stefan     (501) staff       (20)     6055 2023-06-08 12:49:26.000000 sgdml-1.0.1/scripts/sgdml_dataset_via_ase.py
+-rwxr-xr-x   0 stefan     (501) staff       (20)     3388 2023-06-08 12:49:26.000000 sgdml-1.0.1/scripts/sgdml_datasets_from_model.py
+-rw-r--r--   0 stefan     (501) staff       (20)      316 2023-06-08 12:53:02.214817 sgdml-1.0.1/setup.cfg
+-rw-r--r--   0 stefan     (501) staff       (20)     2004 2023-06-08 12:49:26.000000 sgdml-1.0.1/setup.py
+drwxr-xr-x   0 stefan     (501) staff       (20)        0 2023-06-08 12:53:02.212548 sgdml-1.0.1/sgdml/
+-rw-r--r--   0 stefan     (501) staff       (20)     3591 2023-06-08 12:49:26.000000 sgdml-1.0.1/sgdml/__init__.py
+-rw-r--r--   0 stefan     (501) staff       (20)    74967 2023-06-08 12:49:26.000000 sgdml-1.0.1/sgdml/cli.py
+-rwxr-xr-x   0 stefan     (501) staff       (20)     5223 2023-06-08 12:49:26.000000 sgdml-1.0.1/sgdml/get.py
+drwxr-xr-x   0 stefan     (501) staff       (20)        0 2023-06-08 12:53:02.213553 sgdml-1.0.1/sgdml/intf/
+-rwxr-xr-x   0 stefan     (501) staff       (20)        0 2023-06-08 12:49:26.000000 sgdml-1.0.1/sgdml/intf/__init__.py
+-rwxr-xr-x   0 stefan     (501) staff       (20)     4188 2023-06-08 12:49:26.000000 sgdml-1.0.1/sgdml/intf/ase_calc.py
+-rw-r--r--   0 stefan     (501) staff       (20)    46891 2023-06-08 12:49:26.000000 sgdml-1.0.1/sgdml/predict.py
+drwxr-xr-x   0 stefan     (501) staff       (20)        0 2023-06-08 12:53:02.213866 sgdml-1.0.1/sgdml/solvers/
+-rwxr-xr-x   0 stefan     (501) staff       (20)        0 2023-06-08 12:49:26.000000 sgdml-1.0.1/sgdml/solvers/__init__.py
+-rwxr-xr-x   0 stefan     (501) staff       (20)     5423 2023-06-08 12:49:26.000000 sgdml-1.0.1/sgdml/solvers/analytic.py
+-rw-r--r--   0 stefan     (501) staff       (20)    28082 2023-06-08 12:49:26.000000 sgdml-1.0.1/sgdml/solvers/iterative.py
+-rw-r--r--   0 stefan     (501) staff       (20)    40518 2023-06-08 12:49:26.000000 sgdml-1.0.1/sgdml/torchtools.py
+-rw-r--r--   0 stefan     (501) staff       (20)    60606 2023-06-08 12:49:26.000000 sgdml-1.0.1/sgdml/train.py
+drwxr-xr-x   0 stefan     (501) staff       (20)        0 2023-06-08 12:53:02.214446 sgdml-1.0.1/sgdml/utils/
+-rwxr-xr-x   0 stefan     (501) staff       (20)        0 2023-06-08 12:49:26.000000 sgdml-1.0.1/sgdml/utils/__init__.py
+-rw-r--r--   0 stefan     (501) staff       (20)    17340 2023-06-08 12:49:26.000000 sgdml-1.0.1/sgdml/utils/desc.py
+-rwxr-xr-x   0 stefan     (501) staff       (20)    19139 2023-06-08 12:49:26.000000 sgdml-1.0.1/sgdml/utils/io.py
+-rwxr-xr-x   0 stefan     (501) staff       (20)    31377 2023-06-08 12:49:26.000000 sgdml-1.0.1/sgdml/utils/perm.py
+-rwxr-xr-x   0 stefan     (501) staff       (20)    13361 2023-06-08 12:49:26.000000 sgdml-1.0.1/sgdml/utils/ui.py
+drwxr-xr-x   0 stefan     (501) staff       (20)        0 2023-06-08 12:53:02.213358 sgdml-1.0.1/sgdml.egg-info/
+-rw-r--r--   0 stefan     (501) staff       (20)     4567 2023-06-08 12:53:02.000000 sgdml-1.0.1/sgdml.egg-info/PKG-INFO
+-rw-r--r--   0 stefan     (501) staff       (20)      791 2023-06-08 12:53:02.000000 sgdml-1.0.1/sgdml.egg-info/SOURCES.txt
+-rw-r--r--   0 stefan     (501) staff       (20)        1 2023-06-08 12:53:02.000000 sgdml-1.0.1/sgdml.egg-info/dependency_links.txt
+-rw-r--r--   0 stefan     (501) staff       (20)       68 2023-06-08 12:53:02.000000 sgdml-1.0.1/sgdml.egg-info/entry_points.txt
+-rw-r--r--   0 stefan     (501) staff       (20)        1 2023-06-08 12:51:58.000000 sgdml-1.0.1/sgdml.egg-info/not-zip-safe
+-rw-r--r--   0 stefan     (501) staff       (20)       71 2023-06-08 12:53:02.000000 sgdml-1.0.1/sgdml.egg-info/requires.txt
+-rw-r--r--   0 stefan     (501) staff       (20)        6 2023-06-08 12:53:02.000000 sgdml-1.0.1/sgdml.egg-info/top_level.txt
```

### Comparing `sgdml-1.0.0/README.md` & `sgdml-1.0.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -122,10 +122,10 @@
 
 * [3] Chmiela, S., Sauceda, H. E., Poltavsky, I., Müller, K.-R., Tkatchenko, A.,
 *sGDML: Constructing Accurate and Data Efficient Molecular Force Fields Using Machine Learning.*
 Computer Physics Communications, 240, 38-45 (2019)
 [10.1016/j.cpc.2019.02.007](https://doi.org/10.1016/j.cpc.2019.02.007)
 
 * [4] Chmiela, S., Vassilev-Galindo, V., Unke, O. T., Kabylda, A., Sauceda, H. E., Tkatchenko, A., Müller, K.-R.,
-*Accurate global machine learning force fields for molecules with hundreds of atoms.*
-Science Advances, in press, (2022)
-[arXiv:2209.14865](https://arxiv.org/abs/2209.14865)
+*Accurate Global Machine Learning Force Fields for Molecules With Hundreds of Atoms.*
+Science Advances, 9(2), e1603015 (2023)
+[10.1126/sciadv.adf0873](https://doi.org/10.1126/sciadv.adf0873)
```

### Comparing `sgdml-1.0.0/scripts/sgdml_dataset_from_aims.py` & `sgdml-1.0.1/scripts/sgdml_dataset_from_aims.py`

 * *Files identical despite different names*

### Comparing `sgdml-1.0.0/scripts/sgdml_dataset_from_extxyz.py` & `sgdml-1.0.1/scripts/sgdml_dataset_from_extxyz.py`

 * *Files identical despite different names*

### Comparing `sgdml-1.0.0/scripts/sgdml_dataset_from_ipi.py` & `sgdml-1.0.1/scripts/sgdml_dataset_from_ipi.py`

 * *Files identical despite different names*

### Comparing `sgdml-1.0.0/scripts/sgdml_dataset_to_extxyz.py` & `sgdml-1.0.1/scripts/sgdml_dataset_to_extxyz.py`

 * *Files identical despite different names*

### Comparing `sgdml-1.0.0/scripts/sgdml_dataset_via_ase.py` & `sgdml-1.0.1/scripts/sgdml_dataset_via_ase.py`

 * *Files identical despite different names*

### Comparing `sgdml-1.0.0/scripts/sgdml_datasets_from_model.py` & `sgdml-1.0.1/scripts/sgdml_datasets_from_model.py`

 * *Files identical despite different names*

### Comparing `sgdml-1.0.0/setup.py` & `sgdml-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `sgdml-1.0.0/sgdml/__init__.py` & `sgdml-1.0.1/sgdml/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-__version__ = '1.0.0'
+__version__ = '1.0.1'
 
 MAX_PRINT_WIDTH = 100
 LOG_LEVELNAME_WIDTH = 7  # do not modify
 
 # more descriptive callback status
 DONE = 1
 NOT_DONE = 0
```

### Comparing `sgdml-1.0.0/sgdml/cli.py` & `sgdml-1.0.1/sgdml/cli.py`

 * *Files identical despite different names*

### Comparing `sgdml-1.0.0/sgdml/get.py` & `sgdml-1.0.1/sgdml/get.py`

 * *Files identical despite different names*

### Comparing `sgdml-1.0.0/sgdml/intf/ase_calc.py` & `sgdml-1.0.1/sgdml/intf/ase_calc.py`

 * *Files identical despite different names*

### Comparing `sgdml-1.0.0/sgdml/predict.py` & `sgdml-1.0.1/sgdml/predict.py`

 * *Files identical despite different names*

### Comparing `sgdml-1.0.0/sgdml/solvers/analytic.py` & `sgdml-1.0.1/sgdml/solvers/analytic.py`

 * *Files identical despite different names*

### Comparing `sgdml-1.0.0/sgdml/solvers/iterative.py` & `sgdml-1.0.1/sgdml/solvers/iterative.py`

 * *Files identical despite different names*

### Comparing `sgdml-1.0.0/sgdml/torchtools.py` & `sgdml-1.0.1/sgdml/torchtools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 
 # MIT License
 #
-# Copyright (c) 2019-2022 Stefan Chmiela, Jan Hermann
+# Copyright (c) 2019-2023 Stefan Chmiela, Jan Hermann
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -1028,15 +1028,15 @@
         # diffs: N, a, a, 3
         # xs: # N, d
         # x_dists: # N, n_perms*N
         # dot_x_diff_Jx_alphas: N, n_perms*N
         # exp_xs_1_x_dists: N, n_perms*N
         # Fs_x: N, d
 
-        Fs = torch.einsum('ji,...ik,...i->...jk', self.agg_mat, Jxs, Fs_x)
+        Fs = torch.einsum('ji,...ik,...i->...jk', self.agg_mat.double(), Jxs, Fs_x)
 
         if not is_train_pred:  # TODO: set std to zero in training mode?
             Fs *= self._std
 
         if return_E:
             Es *= self._std
             Es += self._c
```

### Comparing `sgdml-1.0.0/sgdml/train.py` & `sgdml-1.0.1/sgdml/train.py`

 * *Files identical despite different names*

### Comparing `sgdml-1.0.0/sgdml/utils/desc.py` & `sgdml-1.0.1/sgdml/utils/desc.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,15 +260,15 @@
 
         # Size of the resulting descriptor vector.
         self.dim = (n_atoms * (n_atoms - 1)) // 2
 
         self.tril_indices = np.tril_indices(n_atoms, k=-1)
 
         # Precompute indices for nonzero entries in desriptor derivatives.
-        self.d_desc_mask = np.zeros((n_atoms, n_atoms - 1), dtype=np.int)
+        self.d_desc_mask = np.zeros((n_atoms, n_atoms - 1), dtype=int)
         for a in range(n_atoms):  # for each partial derivative
             rows, cols = self.tril_indices
             self.d_desc_mask[a, :] = np.concatenate(
                 [np.where(rows == a)[0], np.where(cols == a)[0]]
             )
 
         self.dim_range = np.arange(self.dim)  # [0, 1, ..., dim-1]
```

### Comparing `sgdml-1.0.0/sgdml/utils/io.py` & `sgdml-1.0.1/sgdml/utils/io.py`

 * *Files identical despite different names*

### Comparing `sgdml-1.0.0/sgdml/utils/perm.py` & `sgdml-1.0.1/sgdml/utils/perm.py`

 * *Files identical despite different names*

### Comparing `sgdml-1.0.0/sgdml/utils/ui.py` & `sgdml-1.0.1/sgdml/utils/ui.py`

 * *Files identical despite different names*

### Comparing `sgdml-1.0.0/sgdml.egg-info/SOURCES.txt` & `sgdml-1.0.1/sgdml.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.txt
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 scripts/sgdml_dataset_from_aims.py
 scripts/sgdml_dataset_from_extxyz.py
 scripts/sgdml_dataset_from_ipi.py
```

