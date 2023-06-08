# Comparing `tmp/MDbrew-2.3.3.tar.gz` & `tmp/MDbrew-2.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MDbrew-2.3.3.tar", last modified: Thu May 11 12:13:06 2023, max compression
+gzip compressed data, was "MDbrew-2.3.5.tar", last modified: Thu Jun  8 02:56:52 2023, max compression
```

## Comparing `MDbrew-2.3.3.tar` & `MDbrew-2.3.5.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-11 12:13:06.053016 MDbrew-2.3.3/
--rw-r--r--   0 minu       (501) staff       (20)       25 2023-05-08 12:21:50.000000 MDbrew-2.3.3/MANIFEST.in
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-11 12:13:06.049231 MDbrew-2.3.3/MDbrew/
--rw-r--r--   0 minu       (501) staff       (20)      182 2023-05-11 12:11:55.000000 MDbrew-2.3.3/MDbrew/__init__.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-11 12:13:06.050440 MDbrew-2.3.3/MDbrew/analysis/
--rw-r--r--   0 minu       (501) staff       (20)        0 2023-05-11 12:11:55.000000 MDbrew-2.3.3/MDbrew/analysis/__init__.py
--rw-r--r--   0 minu       (501) staff       (20)     4477 2023-05-11 12:11:55.000000 MDbrew-2.3.3/MDbrew/analysis/msd.py
--rw-r--r--   0 minu       (501) staff       (20)     5984 2023-05-11 12:11:55.000000 MDbrew-2.3.3/MDbrew/analysis/rdf.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-11 12:13:06.050992 MDbrew-2.3.3/MDbrew/application/
--rw-r--r--   0 minu       (501) staff       (20)       30 2023-05-11 12:11:55.000000 MDbrew-2.3.3/MDbrew/application/__init__.py
--rw-r--r--   0 minu       (501) staff       (20)    10054 2023-05-11 12:11:55.000000 MDbrew-2.3.3/MDbrew/application/cp2k2npy.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-11 12:13:06.051433 MDbrew-2.3.3/MDbrew/main/
--rw-r--r--   0 minu       (501) staff       (20)        0 2023-05-11 12:11:55.000000 MDbrew-2.3.3/MDbrew/main/__init__.py
--rw-r--r--   0 minu       (501) staff       (20)     5142 2023-05-11 12:11:55.000000 MDbrew-2.3.3/MDbrew/main/brewery.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-11 12:13:06.052283 MDbrew-2.3.3/MDbrew/main/filetype/
--rw-r--r--   0 minu       (501) staff       (20)        0 2023-05-11 12:11:55.000000 MDbrew-2.3.3/MDbrew/main/filetype/__init__.py
--rw-r--r--   0 minu       (501) staff       (20)      940 2023-05-11 12:11:55.000000 MDbrew-2.3.3/MDbrew/main/filetype/gro.py
--rw-r--r--   0 minu       (501) staff       (20)      904 2023-05-11 12:11:55.000000 MDbrew-2.3.3/MDbrew/main/filetype/lmps.py
--rw-r--r--   0 minu       (501) staff       (20)      848 2023-05-11 12:11:55.000000 MDbrew-2.3.3/MDbrew/main/filetype/pdb.py
--rw-r--r--   0 minu       (501) staff       (20)     4294 2023-05-11 12:11:55.000000 MDbrew-2.3.3/MDbrew/main/filetype/trr.py
--rw-r--r--   0 minu       (501) staff       (20)     1414 2023-05-11 12:11:55.000000 MDbrew-2.3.3/MDbrew/main/filetype/vasp.py
--rw-r--r--   0 minu       (501) staff       (20)      530 2023-05-11 12:11:55.000000 MDbrew-2.3.3/MDbrew/main/filetype/xyz.py
--rw-r--r--   0 minu       (501) staff       (20)     1381 2023-05-11 12:11:55.000000 MDbrew-2.3.3/MDbrew/main/opener.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-11 12:13:06.052873 MDbrew-2.3.3/MDbrew/tool/
--rw-r--r--   0 minu       (501) staff       (20)        0 2023-05-11 12:11:55.000000 MDbrew-2.3.3/MDbrew/tool/__init__.py
--rw-r--r--   0 minu       (501) staff       (20)     3618 2023-05-11 12:11:55.000000 MDbrew-2.3.3/MDbrew/tool/colorfont.py
--rw-r--r--   0 minu       (501) staff       (20)     1578 2023-05-11 12:11:55.000000 MDbrew-2.3.3/MDbrew/tool/decorator.py
--rw-r--r--   0 minu       (501) staff       (20)      765 2023-05-11 12:11:55.000000 MDbrew-2.3.3/MDbrew/tool/doctor.py
--rw-r--r--   0 minu       (501) staff       (20)      619 2023-05-11 12:11:55.000000 MDbrew-2.3.3/MDbrew/tool/spacer.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-11 12:13:06.050024 MDbrew-2.3.3/MDbrew.egg-info/
--rw-r--r--   0 minu       (501) staff       (20)      340 2023-05-11 12:13:05.000000 MDbrew-2.3.3/MDbrew.egg-info/PKG-INFO
--rw-r--r--   0 minu       (501) staff       (20)      740 2023-05-11 12:13:05.000000 MDbrew-2.3.3/MDbrew.egg-info/SOURCES.txt
--rw-r--r--   0 minu       (501) staff       (20)        1 2023-05-11 12:13:05.000000 MDbrew-2.3.3/MDbrew.egg-info/dependency_links.txt
--rw-r--r--   0 minu       (501) staff       (20)        1 2023-05-11 12:13:05.000000 MDbrew-2.3.3/MDbrew.egg-info/not-zip-safe
--rw-r--r--   0 minu       (501) staff       (20)        7 2023-05-11 12:13:05.000000 MDbrew-2.3.3/MDbrew.egg-info/top_level.txt
--rw-r--r--   0 minu       (501) staff       (20)      340 2023-05-11 12:13:06.053073 MDbrew-2.3.3/PKG-INFO
--rw-r--r--   0 minu       (501) staff       (20)       62 2023-05-08 12:21:50.000000 MDbrew-2.3.3/requirement.txt
--rw-r--r--   0 minu       (501) staff       (20)       79 2023-05-11 12:13:06.053269 MDbrew-2.3.3/setup.cfg
--rw-r--r--   0 minu       (501) staff       (20)      664 2023-05-11 12:12:27.000000 MDbrew-2.3.3/setup.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-06-08 02:56:52.964977 MDbrew-2.3.5/
+-rw-r--r--   0 minu       (501) staff       (20)       25 2023-05-08 12:21:50.000000 MDbrew-2.3.5/MANIFEST.in
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-06-08 02:56:52.960544 MDbrew-2.3.5/MDbrew/
+-rw-r--r--   0 minu       (501) staff       (20)      182 2023-06-08 02:56:05.000000 MDbrew-2.3.5/MDbrew/__init__.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-06-08 02:56:52.961979 MDbrew-2.3.5/MDbrew/analysis/
+-rw-r--r--   0 minu       (501) staff       (20)        0 2023-06-08 02:56:05.000000 MDbrew-2.3.5/MDbrew/analysis/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)     4477 2023-06-08 02:56:05.000000 MDbrew-2.3.5/MDbrew/analysis/msd.py
+-rw-r--r--   0 minu       (501) staff       (20)     6171 2023-06-08 02:56:05.000000 MDbrew-2.3.5/MDbrew/analysis/rdf.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-06-08 02:56:52.962405 MDbrew-2.3.5/MDbrew/application/
+-rw-r--r--   0 minu       (501) staff       (20)       20 2023-06-08 02:56:05.000000 MDbrew-2.3.5/MDbrew/application/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)    10136 2023-06-08 02:56:05.000000 MDbrew-2.3.5/MDbrew/application/cp2k.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-06-08 02:56:52.963222 MDbrew-2.3.5/MDbrew/main/
+-rw-r--r--   0 minu       (501) staff       (20)        0 2023-06-08 02:56:05.000000 MDbrew-2.3.5/MDbrew/main/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)     5668 2023-06-08 02:56:05.000000 MDbrew-2.3.5/MDbrew/main/brewery.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-06-08 02:56:52.964193 MDbrew-2.3.5/MDbrew/main/filetype/
+-rw-r--r--   0 minu       (501) staff       (20)        0 2023-06-08 02:56:05.000000 MDbrew-2.3.5/MDbrew/main/filetype/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)      940 2023-06-08 02:56:05.000000 MDbrew-2.3.5/MDbrew/main/filetype/gro.py
+-rw-r--r--   0 minu       (501) staff       (20)      904 2023-06-08 02:56:05.000000 MDbrew-2.3.5/MDbrew/main/filetype/lmps.py
+-rw-r--r--   0 minu       (501) staff       (20)      848 2023-06-08 02:56:05.000000 MDbrew-2.3.5/MDbrew/main/filetype/pdb.py
+-rw-r--r--   0 minu       (501) staff       (20)     4427 2023-06-08 02:56:05.000000 MDbrew-2.3.5/MDbrew/main/filetype/trr.py
+-rw-r--r--   0 minu       (501) staff       (20)     1414 2023-06-08 02:56:05.000000 MDbrew-2.3.5/MDbrew/main/filetype/vasp.py
+-rw-r--r--   0 minu       (501) staff       (20)     1094 2023-06-08 02:56:05.000000 MDbrew-2.3.5/MDbrew/main/filetype/xyz.py
+-rw-r--r--   0 minu       (501) staff       (20)     1695 2023-06-08 02:56:05.000000 MDbrew-2.3.5/MDbrew/main/opener.py
+-rw-r--r--   0 minu       (501) staff       (20)      770 2023-06-08 02:56:05.000000 MDbrew-2.3.5/MDbrew/main/writer.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-06-08 02:56:52.964849 MDbrew-2.3.5/MDbrew/tool/
+-rw-r--r--   0 minu       (501) staff       (20)        0 2023-06-08 02:56:05.000000 MDbrew-2.3.5/MDbrew/tool/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)     3618 2023-06-08 02:56:05.000000 MDbrew-2.3.5/MDbrew/tool/colorfont.py
+-rw-r--r--   0 minu       (501) staff       (20)     1578 2023-06-08 02:56:05.000000 MDbrew-2.3.5/MDbrew/tool/decorator.py
+-rw-r--r--   0 minu       (501) staff       (20)      765 2023-06-08 02:56:05.000000 MDbrew-2.3.5/MDbrew/tool/doctor.py
+-rw-r--r--   0 minu       (501) staff       (20)      695 2023-06-08 02:56:05.000000 MDbrew-2.3.5/MDbrew/tool/spacer.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-06-08 02:56:52.961485 MDbrew-2.3.5/MDbrew.egg-info/
+-rw-r--r--   0 minu       (501) staff       (20)      340 2023-06-08 02:56:52.000000 MDbrew-2.3.5/MDbrew.egg-info/PKG-INFO
+-rw-r--r--   0 minu       (501) staff       (20)      758 2023-06-08 02:56:52.000000 MDbrew-2.3.5/MDbrew.egg-info/SOURCES.txt
+-rw-r--r--   0 minu       (501) staff       (20)        1 2023-06-08 02:56:52.000000 MDbrew-2.3.5/MDbrew.egg-info/dependency_links.txt
+-rw-r--r--   0 minu       (501) staff       (20)        1 2023-05-11 12:13:05.000000 MDbrew-2.3.5/MDbrew.egg-info/not-zip-safe
+-rw-r--r--   0 minu       (501) staff       (20)        7 2023-06-08 02:56:52.000000 MDbrew-2.3.5/MDbrew.egg-info/top_level.txt
+-rw-r--r--   0 minu       (501) staff       (20)      340 2023-06-08 02:56:52.965057 MDbrew-2.3.5/PKG-INFO
+-rw-r--r--   0 minu       (501) staff       (20)       62 2023-05-08 12:21:50.000000 MDbrew-2.3.5/requirement.txt
+-rw-r--r--   0 minu       (501) staff       (20)       79 2023-06-08 02:56:52.965317 MDbrew-2.3.5/setup.cfg
+-rw-r--r--   0 minu       (501) staff       (20)      664 2023-06-08 02:56:37.000000 MDbrew-2.3.5/setup.py
```

### Comparing `MDbrew-2.3.3/MDbrew/analysis/msd.py` & `MDbrew-2.3.5/MDbrew/analysis/msd.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.3/MDbrew/analysis/rdf.py` & `MDbrew-2.3.5/MDbrew/analysis/rdf.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,28 +21,29 @@
         layer: int = 0,
         r_max: float = None,
         resolution: int = 1000,
         dtype: str = "float32",
     ):
         if type(a) == Brewery:
             self.is_Brewery_type = True
-            self.a = a
-            self.b = b
+            self.a = a.reorder()
+            self.b = b.reorder()
             self.a_number = a.atom_num
             self.b_number = b.atom_num
             self.box_size = a.box_size if box_size is None else box_size
             assert len(self.box_size), "plz set box_size"
         else:
             self.is_Brewery_type = False
-            self.a = check_dimension(a, dim=3)
-            self.b = check_dimension(b, dim=3)
+            self.a = check_dimension(a, dim=3, dtype=dtype)
+            self.b = check_dimension(b, dim=3, dtype=dtype)
             self.a_number = self.a.shape[1]
             self.b_number = self.b.shape[1]
             self.box_size = box_size
 
+        self._dtype = dtype
         self.box_size = np.array(self.box_size, dtype=dtype)
         self.half_box_size = self.box_size * 0.5
 
         self.layer_depth = layer
         self.layer = self.__make_layer()
 
         self.resolution = resolution
@@ -86,19 +87,21 @@
             value, count = np.unique(idx_hist, return_counts=True)
             self.hist_data[value] += count
 
     # Function for get hist
     def _cal_hist_data_with_generator(self, start=0, end=None, step=1):
         self.hist_data = np.zeros(self.resolution)
         _apply_boundary_condition = self.__set_boundary_condition()
+        frange = (
+            self.a.frange(start=start, end=end, step=step)
+            if self.a is self.b
+            else zip(self.a.frange(start=start, end=end, step=step), self.b.frange(start=start, end=end, step=step))
+        )
         frame_num = 0
-        for _ in tqdm(
-            zip(self.a.frange(start=start, end=end, step=step), self.b.frange(start=start, end=end, step=step)),
-            **self.kwrgs_trange,
-        ):
+        for _ in tqdm(frange, **self.kwrgs_trange):
             frame_num += 1
             a_unit = self.a.coords
             b_unit = self.b.coords
             diff_position = get_diff_position(a_unit[:, None, :], b_unit[None, :, :])
             diff_position = _apply_boundary_condition(diff_position=diff_position)
             distance = get_distance(diff_position=diff_position, axis=-1)
             idx_hist = self.__cal_idx_histogram(distance=distance)
@@ -131,25 +134,25 @@
             for j in idx_direction_:
                 for k in idx_direction_:
                     list_direction.append([i, j, k])
         return np.array(list_direction) * self.box_size
 
     # get idx for histogram
     def __cal_idx_histogram(self, distance):
-        idx_hist = (distance / self.dr).astype(np.int64)
+        idx_hist = (distance / self.dr).astype("int32")
         return idx_hist[np.where((0 < idx_hist) & (idx_hist < self.resolution))]
 
     # Calculate the Density Function
     def __cal_rdf_from_hist_data(self):
         r_i = self.radii[1:]
         g_r = np.append(0.0, self.hist_data[1:] / np.square(r_i))
         factor = np.array(
             4.0 * np.pi * self.dr * self.frame_num * self.a_number * self.b_number,
-            dtype=np.float64,
+            dtype=self._dtype,
         )
-        box_volume = np.prod(self.box_size, dtype=np.float64)
+        box_volume = np.prod(self.box_size, dtype=self._dtype)
         return g_r * box_volume / factor
 
     # Function for get coordinate number
     def __cal_cn_from_hist_data(self):
         self.n = self.hist_data / (self.frame_num * self.a_number)
         return np.cumsum(self.n)
```

### Comparing `MDbrew-2.3.3/MDbrew/application/cp2k2npy.py` & `MDbrew-2.3.5/MDbrew/application/cp2k.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from tqdm import tqdm
 from scipy import constants
 from ..main.brewery import Brewery
 from ..tool.colorfont import color
 from ..tool.decorator import color_print
 
 
-class CP2K2NPY(object):
+class BrewCP2k(object):
     tqmd_option = {"ascii": " #"}
     printing_option = {
         "2array": f" #CONVERT  {color.font_yellow}List2Array{color.reset}",
         "2a.u": f" #CONVERT  {color.font_yellow}Atomic Unit{color.reset}",
         "save": f" #SAVE  {color.font_yellow}THE DATA{color.reset}",
         "kind2type": f" #CONVERT  {color.font_yellow}KIND2TYPE{color.reset}",
     }
@@ -74,18 +74,19 @@
         F_energy = len(self._energy_list)
         F_stress = len(self._stress_list) / 3
         F_coords = len(self._coord_list)
         self._num_frame = F_energy
         self._num_atom = len(self._force_list) / F_energy
 
     def delete(self, idx):
-        self._cell_list = np.delete(self._cell_list, idx)
-        self._force_list = np.delete(self._force_list, idx)
-        self._energy_list = np.delete(self._energy_list, idx)
-        self._virial_list = np.delete(self._virial_list, idx)
+        self._cell_list = np.delete(self._cell_list, idx, axis=0)
+        self._force_list = np.delete(self._force_list, idx, axis=0)
+        self._energy_list = np.delete(self._energy_list, idx, axis=0)
+        self._virial_list = np.delete(self._virial_list, idx, axis=0)
+        self._num_frame = len(self._energy_list)
         print(f"DELETE : {idx} is deleted")
 
     @color_print(name=printing_option["save"])
     def save_data(self, folder: str = "./", mode: str = "dpdata"):
         folder = folder if folder[-1] == "/" else folder + "/"
         data_path = os.path.join(folder, "set.000")
         if not os.path.exists(data_path):
@@ -202,23 +203,23 @@
                         kind_iter_on = False
                         self.is_contain_kind = True
                     if kind_iter_on and idx > kind_idx:
                         self._kind_list.append(line.split()[2])
                         continue
 
     @color_print(name=printing_option["2array"])
-    def _change2array(self, data_type: str = "float32"):
+    def _change2array(self, data_type: str = "float64"):
         F = int(self._num_frame)
         N = int(self._num_atom)
         self._stress_list = np.array(self._stress_list).astype(data_type).reshape(F, 3, 3)
         self._force_list = np.array(self._force_list).astype(data_type).reshape(F, N, 3)
         self._cell_list = np.tile(self._cell_list, (self._num_frame, 1)).astype(data_type).reshape(F, 3, 3)
         self._energy_list = np.array(self._energy_list).astype(data_type)
         self._coord_list = np.array(self._coord_list).astype(data_type)
-        self._type_list = np.array(self._type_list).astype("int32")
+        self._type_list = np.array(self._type_list).astype("int64")
 
     @color_print(name=printing_option["2a.u"])
     def _convert_unit(self, verbose: bool = True):
         ELE_CHG = constants.elementary_charge  # Elementary Charge, in C
         HARTREE = constants.value("atomic unit of energy")  # Hartree, in Jole
         BOHR = constants.value("atomic unit of length")  # Bohr, in m
```

### Comparing `MDbrew-2.3.3/MDbrew/main/brewery.py` & `MDbrew-2.3.5/MDbrew/main/brewery.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 import os
 import numpy as np
 import pandas as pd
 from .opener import Opener
+from .writer import Writer
 from .filetype.lmps import lmpsOpener
 from .filetype.pdb import pdbOpener
 from .filetype.vasp import vaspOpener
-from .filetype.xyz import xyzOpener
+from .filetype.xyz import xyzOpener, xyzWriter
 from .filetype.trr import trrOpener
 from ..tool.colorfont import color
 from ..tool.decorator import color_print_verbose
 
 
 class Brewery(object):
     __support_opener__: dict["str":Opener] = {
         "auto": None,
         "pdb": pdbOpener,
         "xyz": xyzOpener,
         "vasp": vaspOpener,
         "lmps": lmpsOpener,
         "trr": trrOpener,
     }
+    __support_writer__: dict["str":Writer] = {
+        "xyz": xyzWriter,
+    }
     __print_option__ = {
         "brewery": f" #OPEN  {color.font_yellow}Brewery {color.reset}",
         "b_brewing": f" #BREW  {color.font_yellow}Some...  {color.reset}",
         "b_coords": f" #BREW  {color.font_yellow}Coords     {color.reset}",
         "b_atominfo": f" #BREW  {color.font_yellow}Atom Info  {color.reset}",
     }
 
@@ -79,28 +83,14 @@
     def frame(self):
         return self._opener.frame
 
     @property
     def next_frame(self):
         self._opener.next_frame()
 
-    @color_print_verbose(name=__print_option__["b_brewing"])
-    def brew(self, cols: list[str] = None, what: str = None, dtype: str = "float32", verbose: bool = True):
-        data = pd.DataFrame(data=self.data, columns=self.columns)
-        data = data.query(self._what) if self._what is not None else data
-        data = data.query(what) if what is not None else data
-        data = data.loc[:, cols] if cols is not None else data
-        return data.to_numpy().astype(dtype=dtype)
-
-    def reset(self):
-        self._opener.reset()
-
-    def order(self, what: str = None):
-        return Brewery(trj_file=self._path, fmt=self._fmt, what=what)
-
     @color_print_verbose(name=__print_option__["brewery"])
     def _set_atom_info(self, verbose: bool = True):
         atom_brew_data = self.brew(cols=self._opener._atom_keyword, dtype=str, verbose=False)
         self.atom_info = np.unique(atom_brew_data, return_counts=True)
         self.atom_kind = self.atom_info[0]
         self.atom_num = np.sum(self.atom_info[1])
 
@@ -122,21 +112,44 @@
         return fmt
 
     def _check_path(self, path, **kwrgs):
         path = os.path.join(os.getcwd(), path)
         assert os.path.isfile(path=path), f"Check your path || not {path}"
         return path
 
+    @color_print_verbose(name=__print_option__["b_brewing"])
+    def brew(self, cols: list[str] = None, what: str = None, dtype: str = "float32", verbose: bool = False):
+        data = pd.DataFrame(data=self.data, columns=self.columns)
+        data = data.query(self._what) if self._what is not None else data
+        data = data.query(what) if what is not None else data
+        data = data.loc[:, cols] if cols is not None else data
+        return data.to_numpy(dtype=dtype)
+
+    def reset(self):
+        self._opener.reset()
+
+    def order(self, what: str = None):
+        return Brewery(trj_file=self._path, fmt=self._fmt, what=what)
+
+    def reorder(self):
+        return Brewery(trj_file=self._path, fmt=self._fmt, what=self._what)
+
     def frange(self, start: int = 0, end: int = None, step: int = 1):
         self.move_frame(num=start)
+        if end != None:
+            assert start < end, "start should be lower than end"
         while True:
             try:
                 if self.frame == end:
                     break
                 if not (self.frame - start) % step:
                     yield self.frame
                 self.next_frame
             except:
                 break
 
     def move_frame(self, num):
         self._opener.skip_frame(num=num)
+
+    def write(self, fmt: str, save_path: str, start: int = 0, end: int = None, step: int = 1):
+        _writer = self.__support_writer__[fmt](save_path, self)
+        _writer.write(start=start, end=end, step=step)
```

### Comparing `MDbrew-2.3.3/MDbrew/main/filetype/gro.py` & `MDbrew-2.3.5/MDbrew/main/filetype/gro.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.3/MDbrew/main/filetype/lmps.py` & `MDbrew-2.3.5/MDbrew/main/filetype/lmps.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.3/MDbrew/main/filetype/pdb.py` & `MDbrew-2.3.5/MDbrew/main/filetype/pdb.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.3/MDbrew/main/filetype/trr.py` & `MDbrew-2.3.5/MDbrew/main/filetype/trr.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,19 +24,14 @@
     "step",
     "nre",
     "time",
     "lambda",
 )
 
 
-def unpack_fmt_and_read_line(file, fmt):
-    size = struct.calcsize(fmt)
-    data = file.read(size)
-    data = struct.unpack(fmt, data)
-    return data
 
 
 def check_double(columns_info):
     key_order = ("box_size", "x_size", "v_size", "f_size")
     size = 0
     for key in key_order:
         if columns_info[key] != 0:
@@ -59,32 +54,33 @@
         self._arrow = ">"
         self._dim = DIM
         self._gro_data = _read_gro_file(gro=kwrgs.pop("gro"), idx=GRO_IDX)
         super().gen_db()
 
     # Abstract data
     def _make_one_frame_data(self, file):
+        self.total_line_num = 0
         self.columns_info = self._make_columns(file=file)
         self.system_data, self.motion_data = self._make_database(file=file)
         self.box_size = np.diagonal(self.system_data["box"])
         self.column = self._transform_columns()
         return self._transform_database(self.motion_data)
 
     def _make_columns(self, file):
-        info = unpack_fmt_and_read_line(file=file, fmt=f"{self._arrow}1i")
-        tnum = unpack_fmt_and_read_line(file=file, fmt=f"{self._arrow}2i")
-        vers = unpack_fmt_and_read_line(file=file, fmt=f"{self._arrow}{tnum[0]-1}s")
+        info = self._unpack_fmt_and_read_line(file=file, fmt=f"{self._arrow}1i")
+        tnum = self._unpack_fmt_and_read_line(file=file, fmt=f"{self._arrow}2i")
+        vers = self._unpack_fmt_and_read_line(file=file, fmt=f"{self._arrow}{tnum[0]-1}s")
         version = vers[0].split(b"\0", 1)[0].decode("utf-8")
         assert info[0] == 1993, "I can not open this file"
         assert version == "GMX_trn_file", ValueError("Unkown format")
-        column_data = unpack_fmt_and_read_line(file=file, fmt=f"{self._arrow}13i")
+        column_data = self._unpack_fmt_and_read_line(file=file, fmt=f"{self._arrow}13i")
         columns_info = {COLUMNS[idx]: data for idx, data in enumerate(column_data)}
         self._is_double = check_double(columns_info=columns_info)
         num_fmt = f"{self._arrow}2d" if self._is_double else f"{self._arrow}2f"
-        num = unpack_fmt_and_read_line(file=file, fmt=num_fmt)
+        num = self._unpack_fmt_and_read_line(file=file, fmt=num_fmt)
         columns_info["time"] = num[0]
         columns_info["lambda"] = num[1]
         return columns_info
 
     def _transform_columns(self):
         column_dict = {"x_size": "", "v_size": "v", "f_size": "f"}
         xyz_list = ["x", "y", "z"]
@@ -114,9 +110,16 @@
         gro_data = self._gro_data
         val_data = np.hstack([val for key, val in motion_data.items()])
         return np.hstack([gro_data, val_data])
 
     def _read_main_data(self, file, idx):
         fmt = f"{self._arrow}{idx * self._dim}"
         fmt += "d" if self._is_double else "f"
-        data = unpack_fmt_and_read_line(file=file, fmt=fmt)
+        data = self._unpack_fmt_and_read_line(file=file, fmt=fmt)
         return np.array(data).reshape([idx, self._dim])
+
+    def _unpack_fmt_and_read_line(self, file, fmt):
+        size = struct.calcsize(fmt)
+        self.total_line_num += size
+        data = file.read(size)
+        data = struct.unpack(fmt, data)
+        return data
```

### Comparing `MDbrew-2.3.3/MDbrew/main/filetype/vasp.py` & `MDbrew-2.3.5/MDbrew/main/filetype/vasp.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.3/MDbrew/main/opener.py` & `MDbrew-2.3.5/MDbrew/main/opener.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,46 +9,55 @@
 
     def __init__(self, path: str, *args, **kwrgs) -> None:
         self.path = path
         self.column = []
         self.box_size = []
         self._atom_keyword = "atom"
 
-    def gen_db(self, frame=0):
-        self.frame = frame - 1
-        self._database = self._generate_database()
-        self.next_frame()
-
-    def reset(self):
-        self.gen_db()
-
     @property
     def database(self):
         return self._database
 
     @property
     def data(self):
         return self._data
 
-    def next_frame(self):
-        self._data = next(self._database)
+    def _skip_the_line(self, file):
+        if self.read_mode == "r":
+            for _ in range(self.skip_head):
+                file.readline()
+        elif self.read_mode == "rb":
+            file.read(self.skip_head)
+        else:
+            raise ValueError("plz input correct read mode")
 
     @abstractmethod
     def _make_one_frame_data(self, file):
         pass
 
     # Generation database
     def _generate_database(self):
         with open(file=self.path, mode=self.read_mode) as file:
-            for _ in range(self.skip_head):
-                file.readline()
+            self._skip_the_line(file=file)
             while True:
                 try:
                     self.frame += 1
                     yield self._make_one_frame_data(file=file)
                 except:
                     break
 
+    def gen_db(self, frame=0):
+        self.frame = frame - 1
+        self._database = self._generate_database()
+        self.next_frame()
+
+    def reset(self):
+        self.gen_db()
+
     def skip_frame(self, num):
         total_skip_line = self.total_line_num * num
         self.skip_head += total_skip_line
         self.gen_db(frame=num)
+        self.skip_head -= total_skip_line
+
+    def next_frame(self):
+        self._data = next(self._database)
```

### Comparing `MDbrew-2.3.3/MDbrew/tool/colorfont.py` & `MDbrew-2.3.5/MDbrew/tool/colorfont.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.3/MDbrew/tool/decorator.py` & `MDbrew-2.3.5/MDbrew/tool/decorator.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.3/MDbrew/tool/doctor.py` & `MDbrew-2.3.5/MDbrew/tool/doctor.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.3/MDbrew.egg-info/SOURCES.txt` & `MDbrew-2.3.5/MDbrew.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,18 +8,19 @@
 MDbrew.egg-info/dependency_links.txt
 MDbrew.egg-info/not-zip-safe
 MDbrew.egg-info/top_level.txt
 MDbrew/analysis/__init__.py
 MDbrew/analysis/msd.py
 MDbrew/analysis/rdf.py
 MDbrew/application/__init__.py
-MDbrew/application/cp2k2npy.py
+MDbrew/application/cp2k.py
 MDbrew/main/__init__.py
 MDbrew/main/brewery.py
 MDbrew/main/opener.py
+MDbrew/main/writer.py
 MDbrew/main/filetype/__init__.py
 MDbrew/main/filetype/gro.py
 MDbrew/main/filetype/lmps.py
 MDbrew/main/filetype/pdb.py
 MDbrew/main/filetype/trr.py
 MDbrew/main/filetype/vasp.py
 MDbrew/main/filetype/xyz.py
```

### Comparing `MDbrew-2.3.3/setup.py` & `MDbrew-2.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="MDbrew",
-    version="2.3.3",
+    version="2.3.5",
     author="Knu",
     author_email="minu928@snu.ac.kr",
     url="https://github.com/MyKnu/MDbrew",
     download_url="https://github.com/MyKnu/MDbrew/install_file/MDbrew-2.3.3.tar.gz",
     install_requies=[
         "numpy>=1.0.0",
         "pandas>=1.0.0",
```

