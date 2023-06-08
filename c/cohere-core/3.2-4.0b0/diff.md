# Comparing `tmp/cohere_core-3.2.tar.gz` & `tmp/cohere_core-4.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cohere_core-3.2.tar", last modified: Wed Oct 19 14:53:31 2022, max compression
+gzip compressed data, was "cohere_core-4.0b0.tar", last modified: Thu Jun  8 15:14:52 2023, max compression
```

## Comparing `cohere_core-3.2.tar` & `cohere_core-4.0b0.tar`

### file list

```diff
@@ -1,38 +1,42 @@
-drwxr-xr-x   0 bfrosik   (1764) xsdsdm    (1354)        0 2022-10-19 14:53:31.496114 cohere_core-3.2/
--rwxr-xr-x   0 bfrosik   (1764) xsdsdm    (1354)     1799 2022-08-30 19:47:45.000000 cohere_core-3.2/LICENSE
--rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)      500 2022-10-19 14:53:31.494113 cohere_core-3.2/PKG-INFO
--rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)     2346 2022-09-30 15:14:26.000000 cohere_core-3.2/README.md
-drwxr-xr-x   0 bfrosik   (1764) xsdsdm    (1354)        0 2022-10-19 14:53:31.346120 cohere_core-3.2/cohere_core/
--rwxr-xr-x   0 bfrosik   (1764) xsdsdm    (1354)       71 2022-08-30 19:47:45.000000 cohere_core-3.2/cohere_core/__init__.py
-drwxr-xr-x   0 bfrosik   (1764) xsdsdm    (1354)        0 2022-10-19 14:53:31.409119 cohere_core-3.2/cohere_core/controller/
--rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)    11294 2022-08-30 19:47:45.000000 cohere_core-3.2/cohere_core/controller/AI_guess.py
--rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)      128 2022-08-30 19:47:45.000000 cohere_core-3.2/cohere_core/controller/__init__.py
--rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)     5829 2022-08-30 19:47:45.000000 cohere_core-3.2/cohere_core/controller/op_flow.py
--rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)    27396 2022-09-22 19:56:23.000000 cohere_core-3.2/cohere_core/controller/phasing.py
--rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)    22534 2022-10-10 23:09:33.000000 cohere_core-3.2/cohere_core/controller/reconstruction_GA.py
--rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)     8347 2022-10-05 19:16:46.000000 cohere_core-3.2/cohere_core/controller/reconstruction_multi.py
--rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)     4704 2022-08-30 19:47:45.000000 cohere_core-3.2/cohere_core/controller/reconstruction_single.py
-drwxr-xr-x   0 bfrosik   (1764) xsdsdm    (1354)        0 2022-10-19 14:53:31.425116 cohere_core-3.2/cohere_core/data/
--rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)       35 2022-08-30 19:47:45.000000 cohere_core-3.2/cohere_core/data/__init__.py
--rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)    15784 2022-08-30 19:47:45.000000 cohere_core-3.2/cohere_core/data/alien_tools.py
--rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)     8276 2022-08-30 19:47:45.000000 cohere_core-3.2/cohere_core/data/standard_preprocess.py
-drwxr-xr-x   0 bfrosik   (1764) xsdsdm    (1354)        0 2022-10-19 14:53:31.451119 cohere_core-3.2/cohere_core/lib/
--rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)        0 2022-08-30 19:47:45.000000 cohere_core-3.2/cohere_core/lib/__init__.py
--rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)     9204 2022-08-30 19:47:45.000000 cohere_core-3.2/cohere_core/lib/aflib.py
--rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)     1899 2022-08-30 19:47:45.000000 cohere_core-3.2/cohere_core/lib/cohlib.py
--rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)     3625 2022-08-30 19:47:45.000000 cohere_core-3.2/cohere_core/lib/cplib.py
--rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)     4047 2022-08-30 19:47:45.000000 cohere_core-3.2/cohere_core/lib/nplib.py
-drwxr-xr-x   0 bfrosik   (1764) xsdsdm    (1354)        0 2022-10-19 14:53:31.487118 cohere_core-3.2/cohere_core/utilities/
--rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)       51 2022-08-30 19:47:45.000000 cohere_core-3.2/cohere_core/utilities/__init__.py
--rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)    12566 2022-08-30 19:47:45.000000 cohere_core-3.2/cohere_core/utilities/config_errors_dict.py
--rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)    43297 2022-08-30 19:47:45.000000 cohere_core-3.2/cohere_core/utilities/config_verifier.py
--rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)    18256 2022-10-05 19:18:50.000000 cohere_core-3.2/cohere_core/utilities/dvc_utils.py
--rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)    15547 2022-08-30 19:47:45.000000 cohere_core-3.2/cohere_core/utilities/utils.py
-drwxr-xr-x   0 bfrosik   (1764) xsdsdm    (1354)        0 2022-10-19 14:53:31.372119 cohere_core-3.2/cohere_core.egg-info/
--rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)      500 2022-10-19 14:53:30.000000 cohere_core-3.2/cohere_core.egg-info/PKG-INFO
--rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)      916 2022-10-19 14:53:31.000000 cohere_core-3.2/cohere_core.egg-info/SOURCES.txt
--rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)        1 2022-10-19 14:53:30.000000 cohere_core-3.2/cohere_core.egg-info/dependency_links.txt
--rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)       39 2022-10-19 14:53:30.000000 cohere_core-3.2/cohere_core.egg-info/requires.txt
--rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)       12 2022-10-19 14:53:30.000000 cohere_core-3.2/cohere_core.egg-info/top_level.txt
--rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)       38 2022-10-19 14:53:31.497116 cohere_core-3.2/setup.cfg
--rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)      798 2022-10-19 14:41:19.000000 cohere_core-3.2/setup.py
+drwxr-xr-x   0 bfrosik   (1764) xsdsdm    (1354)        0 2023-06-08 15:14:52.702247 cohere_core-4.0b0/
+-rwxr-xr-x   0 bfrosik   (1764) xsdsdm    (1354)     1799 2023-06-08 15:02:02.000000 cohere_core-4.0b0/LICENSE
+-rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)      553 2023-06-08 15:14:52.697250 cohere_core-4.0b0/PKG-INFO
+-rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)     2763 2023-06-08 15:02:02.000000 cohere_core-4.0b0/README.md
+drwxr-xr-x   0 bfrosik   (1764) xsdsdm    (1354)        0 2023-06-08 15:14:52.451278 cohere_core-4.0b0/cohere_core/
+-rwxr-xr-x   0 bfrosik   (1764) xsdsdm    (1354)       71 2023-06-08 15:02:02.000000 cohere_core-4.0b0/cohere_core/__init__.py
+drwxr-xr-x   0 bfrosik   (1764) xsdsdm    (1354)        0 2023-06-08 15:14:52.556274 cohere_core-4.0b0/cohere_core/controller/
+-rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)    11294 2023-06-08 15:02:02.000000 cohere_core-4.0b0/cohere_core/controller/AI_guess.py
+-rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)      194 2023-06-08 15:02:02.000000 cohere_core-4.0b0/cohere_core/controller/__init__.py
+-rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)    13511 2023-06-08 15:02:02.000000 cohere_core-4.0b0/cohere_core/controller/features.py
+-rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)     9375 2023-06-08 15:02:02.000000 cohere_core-4.0b0/cohere_core/controller/op_flow.py
+-rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)    29245 2023-06-08 15:02:02.000000 cohere_core-4.0b0/cohere_core/controller/phasing.py
+-rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)    22985 2023-06-08 15:02:02.000000 cohere_core-4.0b0/cohere_core/controller/reconstruction_GA.py
+-rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)     3774 2023-06-08 15:02:02.000000 cohere_core-4.0b0/cohere_core/controller/reconstruction_coupled.py
+-rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)     7146 2023-06-08 15:02:02.000000 cohere_core-4.0b0/cohere_core/controller/reconstruction_multi.py
+-rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)     3620 2023-06-08 15:02:02.000000 cohere_core-4.0b0/cohere_core/controller/reconstruction_single.py
+drwxr-xr-x   0 bfrosik   (1764) xsdsdm    (1354)        0 2023-06-08 15:14:52.596267 cohere_core-4.0b0/cohere_core/data/
+-rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)       35 2023-06-08 15:02:02.000000 cohere_core-4.0b0/cohere_core/data/__init__.py
+-rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)    15784 2023-06-08 15:02:02.000000 cohere_core-4.0b0/cohere_core/data/alien_tools.py
+-rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)        0 2023-06-08 15:02:02.000000 cohere_core-4.0b0/cohere_core/data/auto_prep.py
+-rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)     8276 2023-06-08 15:02:02.000000 cohere_core-4.0b0/cohere_core/data/standard_preprocess.py
+drwxr-xr-x   0 bfrosik   (1764) xsdsdm    (1354)        0 2023-06-08 15:14:52.632256 cohere_core-4.0b0/cohere_core/lib/
+-rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)        0 2023-06-08 15:02:02.000000 cohere_core-4.0b0/cohere_core/lib/__init__.py
+-rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)     9204 2023-06-08 15:02:02.000000 cohere_core-4.0b0/cohere_core/lib/aflib.py
+-rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)     8238 2023-06-08 15:02:02.000000 cohere_core-4.0b0/cohere_core/lib/cohlib.py
+-rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)     4281 2023-06-08 15:02:02.000000 cohere_core-4.0b0/cohere_core/lib/cplib.py
+-rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)     4590 2023-06-08 15:02:02.000000 cohere_core-4.0b0/cohere_core/lib/nplib.py
+-rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)     7748 2023-06-08 15:02:02.000000 cohere_core-4.0b0/cohere_core/lib/torchlib.py
+drwxr-xr-x   0 bfrosik   (1764) xsdsdm    (1354)        0 2023-06-08 15:14:52.689244 cohere_core-4.0b0/cohere_core/utilities/
+-rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)       51 2023-06-08 15:02:02.000000 cohere_core-4.0b0/cohere_core/utilities/__init__.py
+-rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)    13634 2023-06-08 15:02:02.000000 cohere_core-4.0b0/cohere_core/utilities/config_errors_dict.py
+-rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)    56104 2023-06-08 15:02:02.000000 cohere_core-4.0b0/cohere_core/utilities/config_verifier.py
+-rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)    16015 2023-06-08 15:02:02.000000 cohere_core-4.0b0/cohere_core/utilities/dvc_utils.py
+-rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)    15547 2023-06-08 15:02:02.000000 cohere_core-4.0b0/cohere_core/utilities/utils.py
+drwxr-xr-x   0 bfrosik   (1764) xsdsdm    (1354)        0 2023-06-08 15:14:52.493264 cohere_core-4.0b0/cohere_core.egg-info/
+-rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)      553 2023-06-08 15:14:52.000000 cohere_core-4.0b0/cohere_core.egg-info/PKG-INFO
+-rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)     1058 2023-06-08 15:14:52.000000 cohere_core-4.0b0/cohere_core.egg-info/SOURCES.txt
+-rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)        1 2023-06-08 15:14:52.000000 cohere_core-4.0b0/cohere_core.egg-info/dependency_links.txt
+-rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)       28 2023-06-08 15:14:52.000000 cohere_core-4.0b0/cohere_core.egg-info/requires.txt
+-rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)       12 2023-06-08 15:14:52.000000 cohere_core-4.0b0/cohere_core.egg-info/top_level.txt
+-rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)       38 2023-06-08 15:14:52.703243 cohere_core-4.0b0/setup.cfg
+-rw-r--r--   0 bfrosik   (1764) xsdsdm    (1354)      819 2023-06-08 15:03:35.000000 cohere_core-4.0b0/setup.py
```

### Comparing `cohere_core-3.2/LICENSE` & `cohere_core-4.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `cohere_core-3.2/README.md` & `cohere_core-4.0b0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,18 @@
 The cohere package provides tools for reconstruction of image of a nanoscale structures from data obtained using Bragg Coherent Diffraction Imaging technique.
 
 The reconstruction has very good performance, in particular when utilizing GPU. User has a choice to run on cpu or GPU by selecting Python library. Supported libraries: numpy, cupy, arrayfire. The libraries cupy or arrayfire are installed by user. The solution offers concurrent processing for fast reconstruction of multiple starting points. 
 
 Important features:
 - Genetic Algorithm (GA) - powerful feature that can deliver good reconstruction result by using GA principles. Based on research "Three-dimensional imaging of dislocation propagation during crystal growth and dissolution, Supplementary Information" by Jesse N. Clark et. al.
 - Artificial Intelligence initial guess for reconstruction - uses AI to find reconstructed object that is subsequently used as input to further reconstruction. The work is built on the research by Yudong Yao, et. al: "AutoPhaseNN: Unsupervised Physics-aware Deep Learning of 3D Nanoscale Bragg Coherent Diffraction Imaging". 
+A trained model must be provided when using this feature. User can download trained model by clicking the following link
+https://g-29c18.fd635.8443.data.globus.org/cherukara/cohere-trained_model.hdf5
 - AutoAlien1 algorithm - a method to remove aliens by automatic means during standard data preprocessing. Based on work "Removal of spurious data in Bragg coherent diffraction imaging: an algorithm for automated data preprocessing" by Kenley Pelzer et. al.
+- Multipeak - support for an experiment where data is collected for adjacent peaks simultaneously and reconstructing this multipeak scenario. The research is in experimental stage. Implemented by Jason (Nick) Porter.
 
 The tools offer a full solution for reading data, formatting the data, reconstruction, and visualization. Each of the componenet can be utilized independently. The project was implemented for the Advanced Photon Source beamline 34-ID-C and thus the data preparation and data visualization is customized for that specific beamline. The measurements and parameters that are used during the experiment are parsed specifically for the beamline setup. We offer the code, as the community would benefit from it when customizing for own case.
 
 Author(s)
 
 Barbara Frosik - Principal Software Engineer at Argonne National Laboratory
```

### Comparing `cohere_core-3.2/cohere_core/controller/AI_guess.py` & `cohere_core-4.0b0/cohere_core/controller/AI_guess.py`

 * *Files identical despite different names*

### Comparing `cohere_core-3.2/cohere_core/controller/phasing.py` & `cohere_core-4.0b0/cohere_core/controller/phasing.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,134 +6,72 @@
 
 
 """
 cohere_core.phasing
 ===================
 
 Provides phasing capabilities for the Bragg CDI data.
-The software can run code utilizing different library, such as numpy, cupy, arrayfire (cpu, cuda, opencl). User configures the choice depending on hardware and installed software.
+The software can run code utilizing different library, such as numpy and cupy. User configures the choice depending on hardware and installed software.
 
 """
 
 import time
 import os
+from math import pi
+import random
 import importlib
 import cohere_core.utilities.dvc_utils as dvut
 import cohere_core.utilities.utils as ut
 import cohere_core.utilities.config_verifier as ver
 import cohere_core.controller.op_flow as of
+import cohere_core.controller.features as ft
 
 __author__ = "Barbara Frosik"
 __copyright__ = "Copyright (c) 2016, UChicago Argonne, LLC."
 __docformat__ = 'restructuredtext en'
 __all__ = ['reconstruction',
            'Rec']
 
 
-def set_lib(dlib, is_af):
+def set_lib(dlib):
     global devlib
     devlib = dlib
-    dvut.set_lib(devlib, is_af)
+    dvut.set_lib(devlib)
+    ft.set_lib(dlib)
 
 
 def get_norm(arr):
     return devlib.sum(devlib.square(devlib.absolute(arr)))
 
 
-class Pcdi:
-    def __init__(self, params, data, dir=None):
-        self.params = params
-        if dir is None:
-            self.kernel = None
-        else:
-            try:
-                self.kernel = devlib.load(dir + '/coherence.npy')
-            except:
-                self.kernel = None
-
-        self.dims = devlib.dims(data)
-        self.roi_data = dvut.crop_center(devlib.fftshift(data), self.params['pc_LUCY_kernel'])
-        if self.params['pc_normalize']:
-            self.sum_roi_data = devlib.sum(devlib.square(self.roi_data))
-        if self.kernel is None:
-            self.kernel = devlib.full(self.params['pc_LUCY_kernel'], 0.5, dtype=devlib.dtype(data))
-
-    def set_previous(self, abs_amplitudes):
-        self.roi_amplitudes_prev = dvut.crop_center(devlib.fftshift(abs_amplitudes), self.params['pc_LUCY_kernel'])
-
-    def apply_partial_coherence(self, abs_amplitudes):
-        abs_amplitudes_2 = devlib.square(abs_amplitudes)
-        converged_2 = devlib.fftconvolve(abs_amplitudes_2, self.kernel)
-        converged_2 = devlib.where(converged_2 < 0.0, 0.0, converged_2)
-        converged = devlib.sqrt(converged_2)
-        return converged
-
-    def update_partial_coherence(self, abs_amplitudes):
-        roi_amplitudes = dvut.crop_center(devlib.fftshift(abs_amplitudes), self.params['pc_LUCY_kernel'])
-        roi_combined_amp = 2 * roi_amplitudes - self.roi_amplitudes_prev
-        if self.params['pc_normalize']:
-            amplitudes_2 = devlib.square(roi_combined_amp)
-            sum_ampl = devlib.sum(amplitudes_2)
-            ratio = self.sum_roi_data / sum_ampl
-            amplitudes = devlib.sqrt(amplitudes_2 * ratio)
-        else:
-            amplitudes = roi_combined_amp
-
-        if self.params['pc_type'] == "LUCY":
-            self.lucy_deconvolution(devlib.square(amplitudes), devlib.square(self.roi_data),
-                                    self.params['pc_LUCY_iterations'])
-
-    def lucy_deconvolution(self, amplitudes, data, iterations):
-        data_mirror = devlib.flip(data)
-        for i in range(iterations):
-            conv = devlib.fftconvolve(self.kernel, data)
-            devlib.where(conv == 0.0, 1.0, conv)
-            relative_blurr = amplitudes / conv
-            self.kernel = self.kernel * devlib.fftconvolve(relative_blurr, data_mirror)
-        self.kernel = devlib.real(self.kernel)
-        coh_sum = devlib.sum(devlib.absolute(self.kernel))
-        self.kernel = devlib.absolute(self.kernel) / coh_sum
-
-
 class Support:
+    """
+    Support class is a state holder for the support array. It initializes the support at creation time.
+    Features that modify support: shrink wrap, phase modifier, lowpass filter.
+    """
     def __init__(self, params, dims, dir=None):
-        self.params = params
-        self.dims = dims
-
+        # create or get initial support
         if dir is None or not os.path.isfile(dir + '/support.npy'):
             initial_support_area = params['initial_support_area']
             init_support = []
             for i in range(len(initial_support_area)):
                 if type(initial_support_area[0]) == int:
                     init_support.append(initial_support_area[i])
                 else:
                     init_support.append(int(initial_support_area[i] * dims[i]))
             center = devlib.full(init_support, 1)
-            self.support = dvut.pad_around(center, self.dims, 0)
+            self.support = dvut.pad_around(center, dims, 0)
         else:
             self.support = devlib.load(dir + '/support.npy')
 
-        # The sigma can change if resolution trigger is active. When it
-        # changes the distribution has to be recalculated using the given sigma
-        # At some iteration the low resolution become inactive, and the sigma
-        # is set to shrink_wrap_gauss_sigma. The prev_sigma is kept to check if sigma changed
-        # and thus the distribution must be updated
-        self.distribution = None
-        self.prev_sigma = 0
-
     def get_support(self):
         return self.support
 
-    def update_amp(self, ds_image, sigma, threshold):
-        self.support = dvut.shrink_wrap(ds_image, threshold, sigma)
-
-    def update_phase(self, ds_image):
-        phase = devlib.angle(ds_image)
-        phase_condition = (phase > self.params['phm_phase_min']) & (phase < self.params['phm_phase_max'])
-        self.support *= phase_condition
+    def flip(self):
+        self.support = devlib.flip(self.support)
 
 
 class Rec:
     """
     cohere_core.phasing.reconstruction(self, params, data_file)
 
     Class, performs phasing using iterative algorithm.
@@ -142,14 +80,33 @@
         parameters used in reconstruction. Refer to x for parameters description
     data_file : str
         name of file containing data to be reconstructed
 
     """
     __all__ = []
     def __init__(self, params, data_file):
+        self.iter_functions = [self.next,
+                          self.lowpass_filter_trigger,
+                          self.reset_resolution,
+                          self.shrink_wrap_trigger,
+                          self.phm_trigger,
+                          self.to_reciprocal_space,
+                          self.new_func_trigger,
+                          self.pc_trigger,
+                          self.pc_modulus,
+                          self.modulus,
+                          self.set_prev_pc_trigger,
+                          self.to_direct_space,
+                          self.er,
+                          self.hio,
+                          self.new_alg,
+                          self.twin_trigger,
+                          self.average_trigger,
+                          self.progress_trigger]
+
         if 'init_guess' not in params:
             params['init_guess'] = 'random'
         elif params['init_guess'] == 'AI_guess':
             if 'AI_threshold' not in params:
                 params['AI_threshold'] = params['shrink_wrap_threshold']
             if 'AI_sigma' not in params:
                 params['AI_sigma'] = params['shrink_wrap_gauss_sigma']
@@ -157,82 +114,34 @@
             params['reconstructions'] = 1
         if 'hio_beta' not in params:
             params['hio_beta'] = 0.9
         if 'initial_support_area' not in params:
             params['initial_support_area'] = (.5, .5, .5)
         if 'twin_trigger' in params and 'twin_halves' not in params:
             params['twin_halves'] = (0, 0)
-        if 'shrink_wrap_gauss_sigma' not in params:
-            params['shrink_wrap_gauss_sigma'] = 1.0
-        if 'shrink_wrap_threshold' not in params:
-            params['shrink_wrap_threshold'] = 0.1
-        if 'shrink_wrap_trigger' in params:
-            if 'shrink_wrap_type' not in params:
-                params['shrink_wrap_type'] = "GAUSS"
-        if 'phase_support_trigger' in params:
-            if 'phm_phase_min' not in params:
-                params['phm_phase_min'] = -1.57
-            if 'phm_phase_max' not in params:
-                params['phm_phase_max'] = 1.57
         if 'pc_interval' in params and 'pc' in params['algorithm_sequence']:
             self.is_pcdi = True
-            if 'pc_type' not in params:
-                params['pc_type'] = "LUCY"
-            if 'pc_LUCY_iterations' not in params:
-                params['pc_LUCY_iterations'] = 20
-            if 'pc_normalize' not in params:
-                params['pc_normalize'] = True
-            if 'pc_LUCY_kernel' not in params:
-                params['pc_LUCY_kernel'] = (16, 16, 16)
         else:
             self.is_pcdi = False
-        self.ll_sigmas = None
-        self.ll_dets = None
-        if 'resolution_trigger' in params and len(params['resolution_trigger']) == 3:
-            # linespacing the sigmas and dets need a number of iterations
-            # The trigger should have three elements, the last one
-            # meaning the last iteration when the low resolution is
-            # applied. If the trigger does not have the limit,
-            # it is misconfigured, and the trigger will not be
-            # active
-            ll_iter = params['resolution_trigger'][2]
-            if 'shrink_wrap_trigger' not in params and 'lowpass_filter_sw_sigma_range' in params:
-                # The sigmas are used to find support, if the shrink wrap
-                # trigger is not active, it wil not be used
-                sigma_range = params['lowpass_filter_sw_sigma_range']
-                if len(sigma_range) > 0:
-                    first_sigma = sigma_range[0]
-                    if len(sigma_range) == 1:
-                        last_sigma = params['shrink_wrap_gauss_sigma']
-                    else:
-                        last_sigma = sigma_range[1]
-                    params['ll_sigmas'] = [first_sigma + x * (last_sigma - first_sigma) / ll_iter for x in range(ll_iter)]
-            if 'lowpass_filter_range' in params:
-                det_range = params['lowpass_filter_range']
-                if type(det_range) ==int:
-                    det_range = [det_range, 1.0]
-                    params['ll_dets'] = [det_range[0] + x * (det_range[1] - det_range[0]) / ll_iter for x in range(ll_iter)]
-            else:
-                params['ll_dets'] = None
         # finished setting defaults
         self.params = params
         self.data_file = data_file
         self.ds_image = None
         self.need_save_data = False
         self.saved_data = None
 
     def init_dev(self, device_id):
+        os.environ["CUDA_DEVICE_ORDER"] = "PCI_BUS_ID"
         self.dev = device_id
-        if device_id != -1:
-            try:
-                devlib.set_device(device_id)
-            except Exception as e:
-                print(e)
-                print('may need to restart GUI')
-                return -1
+        try:
+            devlib.set_device(device_id)
+        except Exception as e:
+            print(e)
+            print('may need to restart GUI')
+            return -1
         if self.data_file.endswith('tif') or self.data_file.endswith('tiff'):
             try:
                 data_np = ut.read_tif(self.data_file)
                 data = devlib.from_numpy(data_np)
             except Exception as e:
                 print(e)
                 return -1
@@ -241,15 +150,14 @@
                 data = devlib.load(self.data_file)
             except Exception as e:
                 print(e)
                 return -1
         else:
             print('no data file found')
             return -1
-
         # in the formatted data the max is in the center, we want it in the corner, so do fft shift
         self.data = devlib.fftshift(devlib.absolute(data))
         self.dims = devlib.dims(self.data)
         print('data shape', self.dims)
 
         if self.need_save_data:
             self.saved_data = devlib.copy(self.data)
@@ -274,107 +182,114 @@
             # cmd is a tuple containing name of the function, followed by arguments
             cmd = worker_qin.get()
             if cmd == 'done':
                 done = True
             else:
                 if type(cmd) == str:
                     # the function does not have any arguments
-                    ret = functions_dict[cmd]()
+                    try:
+                        ret = functions_dict[cmd]()
+                    except:
+                        print('cought exception')
+                        ret = -3
                 else:
+                    try:
                     # the function name is the first element in the cmd tuple, and the other elements are arguments
-                    ret = functions_dict[cmd[0]](*cmd[1:])
+                        ret = functions_dict[cmd[0]](*cmd[1:])
+                    except:
+                        print('cought exception')
+                        ret = -3
+
                 worker_qout.put(ret)
 
+
     def init(self, dir=None, gen=None):
+        def create_feat_objects(params, feats):
+            if 'shrink_wrap_trigger' in params:
+                self.shrink_wrap_obj = ft.ShrinkWrap(params, feats)
+            if 'phm_trigger' in params:
+                self.phm_obj = ft.PhaseMod(params, feats)
+            if 'lowpass_filter_trigger' in params:
+                self.lowpass_filter_obj = ft.LowPassFilter(params, feats)
+
         if self.ds_image is not None:
             first_run = False
         elif dir is None or not os.path.isfile(dir + '/image.npy'):
             self.ds_image = devlib.random(self.dims, dtype=self.data.dtype)
             first_run = True
         else:
             self.ds_image = devlib.load(dir + '/image.npy')
             first_run = False
-        iter_functions = [self.next,
-                          self.resolution_trigger,
-                          self.reset_resolution,
-                          self.shrink_wrap_trigger,
-                          self.phase_support_trigger,
-                          self.to_reciprocal_space,
-                          self.new_func_trigger,
-                          self.pc_trigger,
-                          self.pc_modulus,
-                          self.modulus,
-                          self.set_prev_pc_trigger,
-                          self.to_direct_space,
-                          self.er,
-                          self.hio,
-                          self.new_alg,
-                          self.twin_trigger,
-                          self.average_trigger,
-                          self.progress_trigger]
 
-        flow_items_list = []
-        for f in iter_functions:
-            flow_items_list.append(f.__name__)
+        self.flow_items_list = [f.__name__ for f in self.iter_functions]
 
-        self.is_pc, flow = of.get_flow_arr(self.params, flow_items_list, gen, first_run)
+        self.is_pc, flow, feats = of.get_flow_arr(self.params, self.flow_items_list, gen, first_run)
+        if flow is None:
+            return -1
 
         self.flow = []
-        (op_no, iter_no) = flow.shape
-        for i in range(iter_no):
+        (op_no, self.iter_no) = flow.shape
+        for i in range(self.iter_no):
             for j in range(op_no):
                 if flow[j, i] == 1:
-                    self.flow.append(iter_functions[j])
+                    self.flow.append(self.iter_functions[j])
 
         self.aver = None
         self.iter = -1
         self.errs = []
         self.gen = gen
         self.prev_dir = dir
-        self.sigma = self.params['shrink_wrap_gauss_sigma']
         self.support_obj = Support(self.params, self.dims, dir)
         if self.is_pc:
-            self.pc_obj = Pcdi(self.params, self.data, dir)
+            self.pc_obj = ft.Pcdi(self.params, self.data, dir)
+        # create the object even if the feature inactive, it will be empty
+        create_feat_objects(self.params, feats)
 
         # for the fast GA the data needs to be saved, as it would be changed by each lr generation
         # for non-fast GA the Rec object is created in each generation with the initial data
         if self.saved_data is not None:
             if self.params['low_resolution_generations'] > self.gen:
-                self.data = devlib.gaussian_filter(self.saved_data, self.params['ga_lowpass_filter_sigmas'][self.gen])
+                self.data = devlib.gaussian_filter(self.saved_data, self.params['ga_lpf_sigmas'][self.gen])
             else:
                 self.data = self.saved_data
         else:
             if self.gen is not None and self.params['low_resolution_generations'] > self.gen:
-                self.data = devlib.gaussian_filter(self.data, self.params['ga_lowpass_filter_sigmas'][self.gen])
+                self.data = devlib.gaussian_filter(self.data, self.params['ga_lpf_sigmas'][self.gen])
 
-        if 'll_sigma' not in self.params or not first_run:
+        if 'lowpass_filter_range' not in self.params or not first_run:
             self.iter_data = self.data
         else:
-            self.iter_data = self.data.copy()
+            self.iter_data = devlib.copy(self.data)
 
         if (first_run):
             max_data = devlib.amax(self.data)
             self.ds_image *= get_norm(self.ds_image) * max_data
 
             # the line below are for testing to set the initial guess to support
             # self.ds_image = devlib.full(self.dims, 1.0) + 1j * devlib.full(self.dims, 1.0)
 
             self.ds_image *= self.support_obj.get_support()
         return 0
 
     def breed(self):
         breed_mode = self.params['ga_breed_modes'][self.gen]
+        if self.prev_dir.endswith('alpha'):
+            alpha_dir = self.prev_dir
+        else:
+            alpha_dir = os.path.dirname(os.path.dirname(self.prev_dir)).replace(os.sep, '/') + '/alpha'
+
         if breed_mode != 'none':
-            self.ds_image = dvut.breed(breed_mode, self.prev_dir, self.ds_image)
-            self.support_obj.params = dvut.shrink_wrap(self.ds_image, self.params['ga_shrink_wrap_thresholds'][self.gen],
-                                                       self.params['ga_shrink_wrap_gauss_sigmas'][self.gen])
+            self.ds_image = dvut.breed(breed_mode, alpha_dir, self.ds_image)
+            self.support_obj.params = dvut.shrink_wrap(self.ds_image, self.params['ga_sw_thresholds'][self.gen],
+                                                       self.params['ga_sw_gauss_sigmas'][self.gen])
         return 0
 
 
     def iterate(self):
+        self.iter = -1
         start_t = time.time()
         for f in self.flow:
             f()
 
         print('iterate took ', (time.time() - start_t), ' sec')
 
         if devlib.hasnan(self.ds_image):
@@ -387,20 +302,24 @@
 
         mx = devlib.amax(devlib.absolute(self.ds_image))
         self.ds_image = self.ds_image / mx
 
         return 0
 
 
-    def save_res(self, save_dir):
+    def save_res(self, save_dir, only_image=False):
         from array import array
 
         if not os.path.exists(save_dir):
             os.makedirs(save_dir)
         devlib.save(save_dir + '/image', self.ds_image)
+
+        if only_image:
+            return 0
+
         devlib.save(save_dir + '/support', self.support_obj.get_support())
         if self.is_pc:
             devlib.save(save_dir + '/coherence', self.pc_obj.kernel)
         errs = array('f', self.errs)
 
         with open(save_dir + "/errors.txt", "w+") as err_f:
             err_f.write('\n'.join(map(str, errs)))
@@ -416,57 +335,48 @@
         return 0
 
 
     def get_metric(self, metric_type):
         return dvut.all_metrics(self.ds_image, self.errs)
         # return dvut.get_metric(self.ds_image, self.errs, metric_type)
 
-
     def next(self):
         self.iter = self.iter + 1
 
-
-    def resolution_trigger(self):
-        if 'll_dets' in self.params:
-            sigmas = [dim * self.params['ll_dets'][self.iter] for dim in self.dims]
-            distribution = devlib.gaussian(self.dims, sigmas)
-            max_el = devlib.amax(distribution)
-            distribution = distribution / max_el
-            data_shifted = devlib.fftshift(self.data)
-            masked = data_shifted * distribution
-            self.iter_data = devlib.fftshift(masked)
-
-        if 'll_sigmas' in self.params:
-            self.sigma = self.params['ll_sigmas'][self.iter]
+    def lowpass_filter_trigger(self):
+        args = (self.data, self.iter, self.ds_image)
+        (self.iter_data, self.support_obj.support) = self.lowpass_filter_obj.apply_trigger(*args)
 
     def reset_resolution(self):
         self.iter_data = self.data
-        self.sigma = self.params['shrink_wrap_gauss_sigma']
 
     def shrink_wrap_trigger(self):
-        self.support_obj.update_amp(self.ds_image, self.sigma, self.params['shrink_wrap_threshold'])
+        args = (self.ds_image,)
+        self.support_obj.support = self.shrink_wrap_obj.apply_trigger(*args)
 
-    def phase_support_trigger(self):
-        self.support_obj.update_phase(self.ds_image)
+    def phm_trigger(self):
+        args = (self.ds_image,)
+        self.support_obj.support *= self.phm_obj.apply_trigger(*args)
 
     def to_reciprocal_space(self):
         self.rs_amplitudes = devlib.ifft(self.ds_image)
 
     def new_func_trigger(self):
+        self.params['new_param'] = 1
         print('in new_func_trigger, new_param', self.params['new_param'])
 
     def pc_trigger(self):
         self.pc_obj.update_partial_coherence(devlib.absolute(self.rs_amplitudes))
 
     def pc_modulus(self):
-        abs_amplitudes = devlib.absolute(self.rs_amplitudes).copy()
+        abs_amplitudes = devlib.absolute(self.rs_amplitudes)
         converged = self.pc_obj.apply_partial_coherence(abs_amplitudes)
         ratio = self.get_ratio(self.iter_data, devlib.absolute(converged))
         error = get_norm(
-            devlib.where((converged > 0.0), (devlib.absolute(converged) - self.iter_data), 0.0)) / get_norm(self.iter_data)
+            devlib.where(devlib.absolute(converged) != 0.0, devlib.absolute(converged) - self.iter_data, 0.0)) / get_norm(self.iter_data)
         self.errs.append(error)
         self.rs_amplitudes *= ratio
 
     def modulus(self):
         ratio = self.get_ratio(self.iter_data, devlib.absolute(self.rs_amplitudes))
         error = get_norm(devlib.where((self.rs_amplitudes != 0), (devlib.absolute(self.rs_amplitudes) - self.iter_data),
                                       0)) / get_norm(self.iter_data)
@@ -488,18 +398,18 @@
         self.ds_image = devlib.where((support > 0), self.ds_image_raw, combined_image)
 
     def new_alg(self):
         self.ds_image = 2.0 * (self.ds_image_raw * self.support_obj.get_support()) - self.ds_image_raw
 
     def twin_trigger(self):
         # TODO this will work only for 3D array, but will the twin be used for 1D or 2D?
-        com = devlib.center_of_mass(self.ds_image)
-        sft = [int(self.dims[i] / 2 - com[i]) for i in range(len(self.dims))]
-        self.ds_image = devlib.shift(self.ds_image, sft)
-        dims = self.ds_image.shape
+        # com = devlib.center_of_mass(devlib.absolute(self.ds_image))
+        # sft = [int(self.dims[i] / 2 - com[i]) for i in range(len(self.dims))]
+        # self.ds_image = devlib.shift(self.ds_image, sft)
+        dims = devlib.dims(self.ds_image)
         half_x = int((dims[0] + 1) / 2)
         half_y = int((dims[1] + 1) / 2)
         if self.params['twin_halves'][0] == 0:
             self.ds_image[half_x:, :, :] = 0
         else:
             self.ds_image[: half_x, :, :] = 0
         if self.params['twin_halves'][1] == 0:
@@ -520,14 +430,186 @@
 
     def get_ratio(self, divident, divisor):
         divisor = devlib.where((divisor != 0.0), divisor, 1.0)
         ratio = divident / divisor
         return ratio
 
 
+class Peak:
+    """
+    Holds parameters related to a peak.
+    """
+
+    def __init__(self, dir_ornt):
+        (self.dir, self.orientation) = dir_ornt
+
+    def set_data(self, G_0):
+        import tifffile as tf
+
+        self.g_vec = devlib.array([0, * self.orientation]) * G_0
+        self.gdotg = devlib.array(devlib.dot(self.g_vec, self.g_vec))
+
+        fn = self.dir + '/phasing_data/data.tif'
+        data_np = tf.imread(fn.replace(os.sep, '/'))
+        data = devlib.from_numpy(data_np)
+
+        # in the formatted data the max is in the center, we want it in the corner, so do fft shift
+        self.data = devlib.fftshift(devlib.absolute(data))
+
+
+class CoupledRec(Rec):
+    """
+    Performs a coupled reconstruction of multiple Bragg peaks using iterative phase retrieval. It alternates between a
+    shared object with a density and atomic displacement field and a working object with an amplitude and phase. The
+    general outline of this process is as follows:
+    1. Initialize the shared object with random values.
+    2. Randomly select a diffraction pattern and corresponding reciprocal lattice vector G from the collected data.
+    3. Set the working object to the projection of the shared object onto G.
+    4. Apply standard phase retrieval techniques to the working object for a set number of iterations.
+    5. Update the G-projection of the shared object to be a weighted average of its current value with the working
+        object.
+    6. Repeat steps 2-5.
+
+    params : dict
+        parameters used in reconstruction. Refer to x for parameters description
+    data_file : str
+        name of file containing data for each peak to be reconstructed
+
+    """
+    __author__ = "Nick Porter"
+    __all__ = []
+
+    def __init__(self, params, peak_dir_orient):
+        super().__init__(params, None)
+
+        self.iter_functions = self.iter_functions + [self.switch_peaks]
+
+        if "switch_peak_trigger" not in params:
+            params["switch_peak_trigger"] = [0, 10]
+        if "mp_max_weight" not in params:
+            params["mp_max_weight"] = 0.9
+        if "mp_taper" not in params:
+            params["mp_taper"] = 0.75
+
+        self.peak_objs = [Peak(dir_ornt) for dir_ornt in peak_dir_orient]
+
+
+    def init_dev(self, device_id):
+        self.dev = device_id
+        if device_id != -1:
+            try:
+                devlib.set_device(device_id)
+            except Exception as e:
+                print(e)
+                print('may need to restart GUI')
+                return -1
+
+        G_0 = 2*pi/self.params["lattice_size"]
+        for or_obj in self.peak_objs:
+            or_obj.set_data(G_0)
+
+        self.num_peaks = len(self.peak_objs)
+        self.pk = 0  # index in list of current peak being reconstructed
+        self.data = self.peak_objs[self.pk].data
+        self.iter_data = self.data
+        self.dims = self.data.shape
+
+        if self.need_save_data:
+            self.saved_data = devlib.copy(self.data)
+            self.need_save_data = False
+
+        return 0
+
+    def init(self, img_dir=None, gen=None):
+        if super().init(img_dir, gen) == -1:
+            return -1
+
+        # Define the shared image
+        self.shared_image = devlib.absolute(self.ds_image[:, :, :, None]) * devlib.array([1, 1, 1, 1])
+        self.rho_hat = devlib.array([1, 0, 0, 0])  # This is the density "unit vector" in the shared object.
+
+        # Define the multipeak projection weighting and tapering
+        coeff = self.params["mp_taper"] / (self.params["mp_taper"] - 1)
+        self.proj_weight = devlib.square(devlib.cos(devlib.linspace(coeff*1.57, 1.57, self.iter_no).clip(0, 2)))
+        self.proj_weight = self.proj_weight * self.params["mp_max_weight"]
+
+        return 0
+
+    def save_res(self, save_dir):
+        from array import array
+
+        self.shared_image = self.shared_image * self.support_obj.get_support()[:, :, :, None]
+        if not os.path.exists(save_dir):
+            os.makedirs(save_dir)
+        devlib.save(save_dir + "/image", self.shared_image)
+        devlib.save(save_dir + "/shared_density", self.shared_image[:, :, :, 0])
+        devlib.save(save_dir + "/shared_u1", self.shared_image[:, :, :, 1])
+        devlib.save(save_dir + "/shared_u2", self.shared_image[:, :, :, 2])
+        devlib.save(save_dir + "/shared_u3", self.shared_image[:, :, :, 3])
+        devlib.save(save_dir + '/support', self.support_obj.get_support())
+
+        errs = array('f', self.errs)
+
+        with open(save_dir + "/errors.txt", "w+") as err_f:
+            err_f.write('\n'.join(map(str, errs)))
+
+        devlib.save(save_dir + '/errors', errs)
+
+        metric = dvut.all_metrics(self.ds_image, self.errs)
+        with open(save_dir + "/metrics.txt", "w+") as f:
+            f.write(str(metric))
+
+        return 0
+
+    def switch_peaks(self):
+        self.to_shared_image()
+        self.pk = random.choice([x for x in range(self.num_peaks) if x not in (self.pk,)])
+        self.iter_data = self.peak_objs[self.pk].data
+        self.to_working_image(self.peak_objs[self.pk])
+
+    def to_shared_image(self):
+        beta = self.proj_weight[self.iter]
+        curr_peak = self.peak_objs[self.pk]
+        old_image = (devlib.dot(self.shared_image, curr_peak.g_vec) / curr_peak.gdotg)[:, :, :, None] * \
+                    curr_peak.g_vec + devlib.dot(self.shared_image, self.rho_hat)[:, :, :, None] * self.rho_hat
+        new_image = (devlib.angle(self.ds_image) / curr_peak.gdotg)[:, :, :, None] * curr_peak.g_vec + \
+                    devlib.absolute(self.ds_image)[:, :, :, None] * self.rho_hat
+        self.shared_image = self.shared_image + beta * (new_image - old_image)
+
+
+    def to_working_image(self, peak_obj):
+        phi = devlib.dot(self.shared_image, peak_obj.g_vec)
+        rho = self.shared_image[:, :, :, 0]
+        self.ds_image = rho * devlib.exp(1j*phi)
+
+    def progress_trigger(self):
+        ornt = self.peak_objs[self.pk].orientation
+        print(f'|  iter {self.iter:>4}  '
+              f'|  [{ornt[0]:>2}, {ornt[1]:>2}, {ornt[2]:>2}]  '
+              f'|  err {self.errs[-1]:0.6f}  '
+              f'|  max {self.shared_image[:, :, :, 0].max():0.5g}'
+              )
+
+    def get_density(self):
+        return self.shared_image[:, :, :, 0]
+
+    def get_distortion(self):
+        return self.shared_image[:, :, :, 1:].swapaxes(3, 2).swapaxes(2, 1).swapaxes(1, 0)
+
+    def flip(self):
+        self.shared_image = devlib.flip(self.shared_image, axis=(0, 1, 2))
+        self.shared_image[:, :, :, 1:] *= -1
+        self.support_obj.flip()
+
+    def shift_to_center(self, ind, cutoff=None):
+        shift_dist = -devlib.array(ind) + (self.dims[0]//2)
+        self.shared_image = devlib.shift(self.shared_image, shift_dist, axis=(0, 1, 2))
+        self.support_obj.support = devlib.shift(self.support_obj.support, shift_dist)
+
+
 def reconstruction(datafile, **kwargs):
     """
     Reconstructs the image from experiment data in datafile according to given parameters. The results: image.npy, support.npy, and errors.npy are saved in 'saved_dir' defined in kwargs, or if not defined, in the directory of datafile.
 
     example of the simplest kwargs parameters:
         - algorithm_sequence ='3*(20*ER+180*HIO)+20*ER'
         - shrink_wrap_trigger = [1, 1]
@@ -561,34 +643,34 @@
             supporting "GAUSS" only. Defines which algorithm to use for shrink wrap.
         shrink_wrap_threshold : float
             only point with relative intensity greater than the threshold are selected
         shrink_wrap_gauss_sigma : float
             used to calculate the Gaussian filter
         initial_support_area : list
             If the values are fractional, the support area will be calculated by multiplying by the data array dimensions. The support will be set to 1s to this dimensions centered.
-        phase_support_trigger : list
+        phm_trigger : list
             defines when to update support array using the parameters below by applaying phase constrain.
         phm_phase_min : float
             point with phase below this value will be removed from support area
         phm_phase_max : float
             point with phase over this value will be removed from support area
         pc_interval : int
             defines iteration interval to update coherence.
         pc_type : str
             partial coherence algorithm. 'LUCY' type is supported.
         pc_LUCY_iterations : int
             number of iterations used in Lucy algorithm
         pc_LUCY_kernel : list
             coherence kernel area.
-        resolution_trigger : list
-            defines when to apply low resolution filter using the parameters below.
-        lowpass_filter_sw_sigma_range : list
-            used when applying low resolution to replace support sigma. The sigmas are linespaced for low resolution iterations from first value to last. If only one number given, the last sigma will default to shrink_wrap_gauss_sigma.
+        lowpass_filter_trigger : list
+            defines when to apply lowpass filter using the parameters below.
+        lowpass_filter_sw_threshold : float
+            used in Gass type shrink wrap when applying lowpass filter.
         lowpass_filter_range : list
-            used when applying low resolution data filter while iterating. The det values are linespaced for low resolution iterations from first value to last. The filter is gauss with sigma of linespaced det. If only one number given, the last det will default to 1.
+            used when applying low resolution data filter while iterating. The values are linespaced for lowpass filter iterations from first value to last. The filter is gauss with sigma of linespaced value. If only one number given, the last value will default to 1.
         average_trigger : list
             defines when to apply averaging. Negative start means it is offset from the last iteration.
         progress_trigger : list of int
             defines when to print info on the console. The info includes current iteration and error.
 
     """
     error_msg = ver.verify('config_rec', kwargs)
@@ -611,15 +693,14 @@
             import cupy as cp
             pkg = 'cp'
         except:
             pkg = 'np'
     if pkg == 'cp':
         devlib = importlib.import_module('cohere_core.lib.cplib').cplib
     elif pkg == 'np':
-        print('np')
         devlib = importlib.import_module('cohere_core.lib.nplib').nplib
     else:
         print('supporting cp and np processing')
         return
     set_lib(devlib, False)
 
     worker = Rec(kwargs, datafile)
@@ -630,15 +711,19 @@
     if worker.init_dev(device[0]) < 0:
         return
 
     if 'continue_dir' in kwargs:
         continue_dir = kwargs['continue_dir']
     else:
         continue_dir = None
-    worker.init(continue_dir)
+    ret_code = worker.init(continue_dir)
+    if ret_code < 0:
+        return
     ret_code = worker.iterate()
+    if ret_code < 0:
+        return
     if 'save_dir' in kwargs:
         save_dir = kwargs['save_dir']
     else:
         save_dir, filename = os.path.split(datafile)
     if ret_code == 0:
-        worker.save_res(save_dir)
+        worker.save_res(save_dir)
```

### Comparing `cohere_core-3.2/cohere_core/controller/reconstruction_GA.py` & `cohere_core-4.0b0/cohere_core/controller/reconstruction_GA.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,39 +24,137 @@
 
 __author__ = "Barbara Frosik"
 __copyright__ = "Copyright (c) 2016, UChicago Argonne, LLC."
 __docformat__ = 'restructuredtext en'
 __all__ = ['reconstruction']
 
 
-def set_lib(pkg, ndim=None):
-    global dvclib
-    if pkg == 'af':
-        if ndim == 1:
-            dvclib = importlib.import_module('cohere_core.lib.aflib').aflib1
-        elif ndim == 2:
-            dvclib = importlib.import_module('cohere_core.lib.aflib').aflib2
-        elif ndim == 3:
-            dvclib = importlib.import_module('cohere_core.lib.aflib').aflib3
+class Tracing:
+    def __init__(self, reconstructions, pars, dir):
+        self.init_dirs = []
+        self.report_tracing = []
+
+        if 'init_guess' not in pars:
+            pars['init_guess'] = 'random'
+        if pars['init_guess'] == 'continue':
+            continue_dir = pars['continue_dir']
+            for sub in os.listdir(continue_dir):
+                image, support, coh = ut.read_results(continue_dir + '/' + sub + '/')
+                if image is not None:
+                    self.init_dirs.append(continue_dir + '/' + sub)
+                    self.report_tracing.append([continue_dir + '/' + sub])
+            if len(self.init_dirs) < reconstructions:
+                for i in range(reconstructions - len(self.init_dirs)):
+                    self.report_tracing.append(['random' + str(i)])
+                self.init_dirs = self.init_dirs + (reconstructions - len(self.init_dirs)) * [None]
+        elif pars['init_guess'] == 'AI_guess':
+            import cohere_core.controller.AI_guess as ai
+
+            self.report_tracing.append(['AI_guess'])
+            for i in range(reconstructions - 1):
+                self.report_tracing.append(['random' + str(i)])
+            # ai_dir = ai.start_AI(pars, datafile, dir)
+            # if ai_dir is None:
+            #     return
+            self.init_dirs = [dir + '/results_AI'] + (reconstructions - 1) * [None]
         else:
-            raise NotImplementedError
-    elif pkg == 'cp':
-        dvclib = importlib.import_module('cohere_core.lib.cplib').cplib
+            for i in range(reconstructions):
+                self.init_dirs.append(None)
+                self.report_tracing.append(['random' + str(i)])
+
+
+    def set_map(self, map):
+        self.map = map
+
+
+    def append_gen(self, gen_ranks):
+        for key in gen_ranks:
+            self.report_tracing[self.map[key]].append(gen_ranks[key])
+
+
+    def pretty_format_results(self):
+        """
+        Takes in a list of report traces and formats them into human-readable tables.
+        Performs data conversion in 1 pass and formatting in a second to determine
+        padding and spacing schemes.
+
+        Parameters
+        ----------
+        none
+
+        Returns
+        -------
+            report_output : str
+            a string containing the formatted report
+        """
+        col_gap = 2
+
+        num_gens = len(self.report_tracing[0]) - 1
+        fitnesses = list(self.report_tracing[0][1][1].keys())
+
+        report_table = []
+        report_table.append(['start'] + [f'generation {i}' for i in range(num_gens)])
+        report_table.append([''] * len(report_table[0]))
+
+        data_col_width = 15
+        start_col_width = 15
+        for pop_data in self.report_tracing:
+            report_table.append([str(pop_data[0])] + [str(ind_data[0]) for ind_data in pop_data[1:]])
+            start_col_width = max(len(pop_data[0]), start_col_width)
+
+            for fit in fitnesses:
+                fit_row = ['']
+                for ind_data in pop_data[1:]:
+                    data_out = f'{fit} : {ind_data[1][fit]}'
+                    data_col_width = max(len(data_out), data_col_width)
+                    fit_row.append(data_out)
+                report_table.append(fit_row)
+            report_table.append([''] * len(report_table[0]))
+
+        report_str = ''
+        for row in report_table:
+            report_str += row[0].ljust(start_col_width + col_gap)
+            report_str += (' ' * col_gap).join([cell.ljust(data_col_width) for cell in row[1:]]) + '\n'
+
+        return report_str
+
+
+    def save(self, save_dir):
+        try:
+            report_str = self.pretty_format_results()
+        except Exception as e:
+            print(f'WARNING: Report formatting failed due to {type(e)}: {e}! Falling back to raw formatting.')
+            report_str = '\n'.join([str(l) for l in self.report_tracing])
+
+        with open(save_dir + '/ranks.txt', 'w+') as rank_file:
+            rank_file.write(report_str)
+            rank_file.flush()
+
+
+def set_lib(pkg):
+    global dvclib
+    if pkg == 'cp':
+        devlib = importlib.import_module('cohere_core.lib.cplib').cplib
     elif pkg == 'np':
-        dvclib = importlib.import_module('cohere_core.lib.nplib').nplib
-    calc.set_lib(dvclib, pkg=='af')
+        devlib = importlib.import_module('cohere_core.lib.nplib').nplib
+    elif pkg == 'torch':
+        devlib = importlib.import_module('cohere_core.lib.torchlib').torchlib
+    calc.set_lib(devlib)
 
 
 def set_ga_defaults(pars):
     if 'reconstructions' not in pars:
         pars['reconstructions'] = 1
 
     if 'ga_generations' not in pars:
         pars['ga_generations'] = 1
 
+    if 'init_guess' not in pars:
+        pars['init_guess'] = 'random'
+
     # check if pc feature is on
     if 'pc' in pars['algorithm_sequence'] and 'pc_interval' in pars:
         if not 'ga_gen_pc_start' in pars:
             pars['ga_gen_pc_start'] = 0
             pars['ga_gen_pc_start'] = min(pars['ga_gen_pc_start'], pars['ga_generations']-1)
 
     if 'ga_fast' not in pars:
@@ -86,103 +184,113 @@
         reconstructions = reconstructions - culling
         if reconstructions <= 0:
             return 'culled down to 0 reconstructions, check configuration'
         ga_reconstructions.append(reconstructions)
     pars['ga_reconstructions'] = ga_reconstructions
 
     if 'shrink_wrap_threshold' in pars:
-        shrink_wrap_threshold = pars['shrink_wrap_threshold']
+        sw_threshold = pars['shrink_wrap_threshold']
     else:
-        shrink_wrap_threshold = .1
-    if 'ga_shrink_wrap_thresholds' in pars:
-        ga_shrink_wrap_thresholds = pars['ga_shrink_wrap_thresholds']
-        if len(ga_shrink_wrap_thresholds) == 1:
-            ga_shrink_wrap_thresholds = ga_shrink_wrap_thresholds * pars['ga_generations']
-        elif len(ga_shrink_wrap_thresholds) < pars['ga_generations']:
-            ga_shrink_wrap_thresholds = ga_shrink_wrap_thresholds + [shrink_wrap_threshold] * (pars['ga_generations'] - len(ga_shrink_wrap_thresholds))
-    else:
-        ga_shrink_wrap_thresholds = [shrink_wrap_threshold] * pars['ga_generations']
-    pars['ga_shrink_wrap_thresholds'] = ga_shrink_wrap_thresholds
-
-    if 'shrink_wrap_gauss_sigma' in pars:
-        shrink_wrap_gauss_sigma = pars['shrink_wrap_gauss_sigma']
-    else:
-        shrink_wrap_gauss_sigma = .1
-    if 'ga_shrink_wrap_gauss_sigmas' in pars:
-        ga_shrink_wrap_gauss_sigmas = pars['ga_shrink_wrap_gauss_sigmas']
-        if len(ga_shrink_wrap_gauss_sigmas) == 1:
-            ga_shrink_wrap_gauss_sigmas = ga_shrink_wrap_gauss_sigmas * pars['ga_generations']
-        elif len(pars['ga_shrink_wrap_gauss_sigmas']) < pars['ga_generations']:
-            ga_shrink_wrap_gauss_sigmas = ga_shrink_wrap_gauss_sigmas + [shrink_wrap_gauss_sigma] * (pars['ga_generations'] - len(ga_shrink_wrap_gauss_sigmas))
+        sw_threshold = .1
+    if 'ga_sw_thresholds' in pars:
+        ga_sw_thresholds = pars['ga_sw_thresholds']
+        if len(ga_sw_thresholds) == 1:
+            ga_sw_thresholds = ga_sw_thresholds * pars['ga_generations']
+        elif len(ga_sw_thresholds) < pars['ga_generations']:
+            ga_sw_thresholds = ga_sw_thresholds + [sw_threshold] * (pars['ga_generations'] - len(ga_sw_thresholds))
+    else:
+        ga_sw_thresholds = [sw_threshold] * pars['ga_generations']
+    pars['ga_sw_thresholds'] = ga_sw_thresholds
+
+    if 'sw_gauss_sigma' in pars:
+        sw_gauss_sigma = pars['sw_gauss_sigma']
+    else:
+        sw_gauss_sigma = .1
+    if 'ga_sw_gauss_sigmas' in pars:
+        ga_sw_gauss_sigmas = pars['ga_sw_gauss_sigmas']
+        if len(ga_sw_gauss_sigmas) == 1:
+            ga_sw_gauss_sigmas = ga_sw_gauss_sigmas * pars['ga_generations']
+        elif len(pars['ga_sw_gauss_sigmas']) < pars['ga_generations']:
+            ga_sw_gauss_sigmas = ga_sw_gauss_sigmas + [sw_gauss_sigma] * (pars['ga_generations'] - len(ga_sw_gauss_sigmas))
     else:
-        ga_shrink_wrap_gauss_sigmas = [shrink_wrap_gauss_sigma] * pars['ga_generations']
-    pars['ga_shrink_wrap_gauss_sigmas'] = ga_shrink_wrap_gauss_sigmas
+        ga_sw_gauss_sigmas = [sw_gauss_sigma] * pars['ga_generations']
+    pars['ga_sw_gauss_sigmas'] = ga_sw_gauss_sigmas
 
     if 'ga_breed_modes' not in pars:
         pars['ga_breed_modes'] = ['sqrt_ab'] * pars['ga_generations']
     else:
         ga_breed_modes = pars['ga_breed_modes']
         if len(ga_breed_modes) == 1:
             ga_breed_modes = ga_breed_modes * pars['ga_generations']
         elif len(ga_breed_modes) < pars['ga_generations']:
             ga_breed_modes = ga_breed_modes + ['sqrt_ab'] * (pars['ga_generations'] - len(ga_breed_modes))
     pars['ga_breed_modes'] = ga_breed_modes
 
-    if 'ga_lowpass_filter_sigmas' in pars:
-        pars['low_resolution_generations'] = len(pars['ga_lowpass_filter_sigmas'])
+    if 'ga_lpf_sigmas' in pars:
+        pars['low_resolution_generations'] = len(pars['ga_lpf_sigmas'])
     else:
         pars['low_resolution_generations'] = 0
 
     if pars['low_resolution_generations'] > 0:
         if 'low_resolution_alg' not in pars:
             pars['low_resolution_alg'] = 'GAUSS'
 
+    print()
+
     return pars
 
 
-def order_dirs(tmp, dirs, evals, metric, first_gen):
+def order_dirs(tracing, dirs, evals, metric_type):
     """
     Orders results in generation directory in subdirectories numbered from 0 and up, the best result stored in the '0' subdirectory. The ranking is done by numbers in evals list, which are the results of the generation's metric to the image array.
 
     Parameters
     ----------
+    tracing : object
+        Tracing object that keeps fields related to tracing
     dirs : list
         list of directories where the reconstruction results files are saved
     evals : list
-        list of evaluation of the results in the directories from the dirs list. The evaluation is a number calculated for metric configured for this generation
+        list of evaluations of the results saved in the directories matching dirs list. The evaluations are dict
+        <metric type> : <eval result>
+    metric_type : metric type to be applied for evaluation
 
     Returns
     -------
-    ordered_prev_dirs : list
-        a list of previous directories ordered from best to worst
+    list :
+        a list of directories where results are saved ordered from best to worst
+    dict :
+        evaluations of the best results
     """
     # ranks keeps indexes of reconstructions from best to worst
     # for most of the metric types the minimum of the metric is best, but for
-    # 'summed_phase' and 'area' it is oposite, so reversing the order
-    metric_evals = [e[metric] for e in evals]
+    # 'summed_phase' and 'area' it is opposite, so reversing the order
+    metric_evals = [e[metric_type] for e in evals]
     ranks = np.argsort(metric_evals).tolist()
-    if metric == 'summed_phase' or metric == 'area':
+    if metric_type == 'summed_phase' or metric_type == 'area':
         ranks.reverse()
     best_metrics = evals[ranks[0]]
-    tracing = {}
-    if first_gen:
-        for i in range(len(ranks)):
-            prev_seq = int(os.path.basename(dirs[ranks[i]]))
-            tmp[prev_seq].append((i, evals[ranks[i]]))
-            tracing[i] = prev_seq
-    else:
-        prev_tracing = tmp.pop()
-        for i in range(len(ranks)):
-            prev_seq = int(os.path.basename(dirs[ranks[i]]))
-            inx = prev_tracing[prev_seq]
-            tmp[inx].append((i, evals[ranks[i]]))
-            tracing[i] = inx
-        prev_tracing.clear()
-    tmp.append(tracing)
 
+    # Add tracing for the generation results
+    gen_ranks = {}
+    for i in range(len(evals)):
+        gen_ranks[ranks[i]] = (i, evals[ranks[i]])
+    tracing.append_gen(gen_ranks)
+
+    # find how the directories based on ranking, map to the initial start
+    prev_map = tracing.map
+    map = {}
+    for i in range(len(ranks)):
+        prev_seq = int(os.path.basename(dirs[ranks[i]]))
+        inx = prev_map[prev_seq]
+        map[i] = inx
+    prev_map.clear()
+    tracing.set_map(map)
+
+    # order directories by rank
     rank_dirs = []
     # append "_<rank>" to each result directory name
     for i in range(len(ranks)):
         dest = dirs[ranks[i]] + '_' + str(i)
         src = dirs[ranks[i]]
         shutil.move(src, dest)
         rank_dirs.append(dest)
@@ -192,111 +300,72 @@
     current_dirs = []
     for dir in rank_dirs:
         last_sub = os.path.basename(dir)
         parent_dir = os.path.dirname(dir).replace(os.sep, '/')
         dest = parent_dir + '/' + last_sub.split('_')[-1]
         shutil.move(dir, dest)
         current_dirs.append(dest)
-    return current_dirs, tmp, best_metrics
+    return current_dirs, best_metrics
 
 
-def order_processes(proc_metrics, metric_type):
+def order_processes(tracing, proc_metrics, metric_type):
     """
     Orders results in generation directory in subdirectories numbered from 0 and up, the best result stored in the '0' subdirectory. The ranking is done by numbers in evals list, which are the results of the generation's metric to the image array.
 
     Parameters
     ----------
-    dirs : list
-        list of directories where the reconstruction results files are saved
-    evals : list
-        list of evaluation of the results in the directories from the dirs list. The evaluation is a number calculated for metric configured for this generation
+    tracing : object
+        Tracing object that keeps fields related to tracing
+    proc_metrics : dict
+        dictionary of <pid> : <evaluations> ; evaluations of the results saved in the directories matching dirs list. The evaluations are dict
+        <metric type> : <eval result>
+    metric_type : metric type to be applied for evaluation
 
     Returns
     -------
-    nothing
+    list :
+        a list of processes ids ordered from best to worst by the results the processes delivered
+    dict :
+        evaluations of the best results
     """
-    ranked_proc = sorted(proc_metrics.items(), key=lambda x: x[1], reverse=False)
+    proc_eval = [(key, proc_metrics[key][metric_type]) for key in proc_metrics.keys()]
+    ranked_proc = sorted(proc_eval, key=lambda x: x[1])
 
-    # ranks keeps indexes of reconstructions from best to worst
+    # ranks keeps indexes of reconstructions from best to worstpro
     # for most of the metric types the minimum of the metric is best, but for
     # 'summed_phase' and 'area' it is oposite, so reversing the order
     if metric_type == 'summed_phase' or metric_type == 'area':
         ranked_proc.reverse()
-    return ranked_proc
+    gen_ranks = {}
+    for i in range(len(ranked_proc)):
+        pid = ranked_proc[i][0]
+        gen_ranks[pid] = (i, proc_metrics[pid])
+    tracing.append_gen(gen_ranks)
+    return ranked_proc, proc_metrics[ranked_proc[0][0]]
 
 
 def cull(lst, no_left):
     if len(lst) <= no_left:
         return lst
     else:
         return lst[0:no_left]
 
 
-def pretty_format_results(report_traces):
-    """
-    Takes in a list of report traces and formats them into human-readable tables.
-    Performs data conversion in 1 pass and formatting in a second to determine
-    padding and spacing schemes. 
-
-    Parameters
-    ----------
-    report_traces: list
-        list of the report trace data structures generated by the GA
-        Assumes report_traces is ordered by order_dirs
-
-    Returns
-    -------
-        report_output : str
-        a string containing the formatted report
-    """
-    col_gap = 2
-
-    num_gens = len(report_traces[0]) - 1
-    fitnesses = list(report_traces[0][1][1].keys())
-
-    report_table = []
-    report_table.append(['start'] + [f'generation {i}' for i in range(num_gens)])
-    report_table.append([''] * len(report_table[0]))
-
-    data_col_width = 15
-    start_col_width = 15
-    for pop_data in report_traces:
-        report_table.append([str(pop_data[0])] + [str(ind_data[0]) for ind_data in pop_data[1:]])
-        start_col_width = max(len(pop_data[0]), start_col_width)
-
-        for fit in fitnesses:
-            fit_row = ['']
-            for ind_data in pop_data[1:]:
-                data_out = f'{fit} : {ind_data[1][fit]}'
-                data_col_width = max(len(data_out), data_col_width)
-                fit_row.append(data_out)
-            report_table.append(fit_row)
-        report_table.append([''] * len(report_table[0]))
-        
-    report_str = ''
-    for row in report_table:
-        report_str += row[0].ljust(start_col_width + col_gap)
-        report_str += (' ' * col_gap).join([cell.ljust(data_col_width) for cell in row[1:]]) + '\n'
-    
-    return report_str
-
 def reconstruction(lib, conf_file, datafile, dir, devices):
     """
     Controls reconstruction that employs genetic algorith (GA).
 
     This script is typically started with cohere_core-ui helper functions. The 'init_guess' parameter in the configuration file defines whether it is a random guess, AI algorithm determined (one reconstruction, the rest random), or starting from some saved state. It will set the initial guess accordingly and start GA algorithm. It will run multiple reconstructions for each generation in a loop. After each generation the best reconstruction, alpha is identified, and used for breeding. For each generation the results will be saved in g_x subdirectory, where x is the generation number, in configured 'save_dir' parameter or in 'results_phasing' subdirectory if 'save_dir' is not defined.
 
     Parameters
     ----------
     lib : str
         library acronym to use for reconstruction. Supported:
         np - to use numpy,
         cp - to use cupy,
-        af - to use arrayfire,
-        cpu, opencl, or cuda - to use specified library of arrayfire
 
     conf_file : str
         configuration file name
 
     datafile : str
         data file name
 
@@ -306,191 +375,170 @@
     devices : list
         list of GPUs available for this reconstructions
 
     """
     pars = ut.read_config(conf_file)
     pars = set_ga_defaults(pars)
 
+    if pars['ga_generations'] < 2:
+        print("number of generations must be greater than 1")
+        return
+
+    if pars['reconstructions'] < 2:
+        print("GA not implemented for a single reconstruction")
+        return
+
+    if pars['ga_fast']:
+        reconstructions = min(pars['reconstructions'], len(devices))
+    else:
+        reconstructions = pars['reconstructions']
+
+    if 'ga_cullings' in pars:
+        cull_sum = sum(pars['ga_cullings'])
+        if reconstructions - cull_sum < 2:
+            print("At least two reconstructions should be left after culling. Number of starting reconstructions is", reconstructions, "but ga_cullings adds to", cull_sum)
+            return
+
+    if pars['init_guess'] == 'AI_guess':
+        # run AI part first
+        import cohere_core.controller.AI_guess as ai
+        ai_dir = ai.start_AI(pars, datafile, dir)
+        if ai_dir is None:
+            return
+
     if 'save_dir' in pars:
         save_dir = pars['save_dir']
     else:
         filename = conf_file.split('/')[-1]
         save_dir = dir + '/' + filename.replace('config_rec', 'results_phasing')
-    generations = pars['ga_generations']
-    if 'reconstructions' in pars:
-        reconstructions = pars['reconstructions']
-    else:
-        reconstructions = 1
 
-    if reconstructions < 2:
-        print ("GA not implemented for a single reconstruction")
-        return
+    # create alpha dir and placeholder for the alpha's metrics
+    alpha_dir = save_dir + '/alpha'
+    if not os.path.isdir(save_dir):
+        os.mkdir(save_dir)
+    if not os.path.isdir(alpha_dir):
+        os.mkdir(alpha_dir)
+
+    tracing = Tracing(reconstructions, pars, dir)
 
-    # the cupy does not run correctly with multiprocessing, but limiting number of runs to available devices will work as temporary fix
     if pars['ga_fast']:  # the number of processes is the same as available GPUs (can be same GPU if can fit more recs)
-        if lib == 'af' or lib == 'cpu' or lib == 'opencl' or lib == 'cuda':
-            if datafile.endswith('tif') or datafile.endswith('tiff'):
-                try:
-                    data = ut.read_tif(datafile)
-                except:
-                    print('could not load data file', datafile)
-                    return
-            elif datafile.endswith('npy'):
-                try:
-                    data = np.load(datafile)
-                except:
-                    print('could not load data file', datafile)
-                    return
-            else:
-                print('no data file found')
-                return
-            set_lib('af', len(data.shape))
-            if lib != 'af':
-                dvclib.set_backend(lib)
-        else:
-            set_lib(lib)
+        set_lib(lib)
 
-        reconstructions = min(reconstructions, len(devices))
-        workers = [calc.Rec(pars, datafile) for _ in range(reconstructions)]
+        workers = []
         processes = {}
+        tracing_map = {}
+        init_dirs = {}
 
-        for worker in workers:
+        for i in range(reconstructions):
+            workers.append(calc.Rec(pars, datafile))
             worker_qin = Queue()
             worker_qout = Queue()
-            process = Process(target=worker.fast_ga, args=(worker_qin, worker_qout))
+            process = Process(target=workers[i].fast_ga, args=(worker_qin, worker_qout))
             process.start()
             processes[process.pid] = [worker_qin, worker_qout]
+            init_dirs[process.pid] = tracing.init_dirs[i]
+            tracing_map[process.pid] = i
+        tracing.set_map(tracing_map)
+
+        def handle_cmd():
+            bad_processes = []
+            for pid in processes:
+                worker_qout = processes[pid][1]
+                ret = worker_qout.get()
+                if ret < 0:
+                    worker_qin = processes[pid][0]
+                    worker_qin.put('done')
+                    bad_processes.append(pid)
+            # remove bad processes from dict (in the future we may reuse them)
+            for pid in bad_processes:
+                processes.pop(pid)
 
-        prev_dirs = None
-        for g in range(generations):
-            print ('starting generation',g)
+        for g in range(pars['ga_generations']):
+            print ('starting generation', g)
             if g == 0:
                 for pid in processes:
                     worker_qin = processes[pid][0]
                     worker_qin.put(('init_dev', devices.pop()))
-                bad_processes = []
+                handle_cmd()
                 for pid in processes:
-                    worker_qout = processes[pid][1]
-                    ret = worker_qout.get()
-                    if ret < 0:
-                        worker_qin = processes[pid][0]
-                        worker_qin.put('done')
-                        bad_processes.append(pid)
-                # remove bad processes from dict (in the future we may reuse them)
-                for pid in bad_processes:
-                    processes.pop(pid)
-            for pid in processes:
-                worker_qin = processes[pid][0]
-                if prev_dirs is None:
-                    prev_dir = None
-                else:
-                    prev_dir = prev_dirs[pid]
-                worker_qin.put(('init', prev_dir, g))
-            for pid in processes:
-                worker_qout = processes[pid][1]
-                ret = worker_qout.get()
+                    worker_qin = processes[pid][0]
+                    worker_qin.put(('init', init_dirs[pid], g))
+                handle_cmd()
+            else:
+                for pid in processes:
+                    worker_qin = processes[pid][0]
+                    worker_qin.put(('init', alpha_dir, g))
+                handle_cmd()
             if g > 0:
                 for pid in processes:
                     worker_qin = processes[pid][0]
                     worker_qin.put('breed')
-                for pid in processes:
-                    worker_qout = processes[pid][1]
-                    ret = worker_qout.get()
+                handle_cmd()
+
             for pid in processes:
                 worker_qin = processes[pid][0]
                 worker_qin.put('iterate')
-            bad_processes = []
-            for pid in processes:
-                worker_qout = processes[pid][1]
-                ret = worker_qout.get()
-                if ret < 0:
-                    worker_qin = processes[pid][0]
-                    worker_qin.put('done')
-                    bad_processes.append(pid)
-            # remove bad processes from dict (in the future we may reuse them)
-            for pid in bad_processes:
-                processes.pop(pid)
+            handle_cmd()
             # get metric, i.e the goodness of reconstruction from each run
             proc_metrics = {}
             metric_type = pars['ga_metrics'][g]
             for pid in processes:
                 worker_qin = processes[pid][0]
                 worker_qin.put(('get_metric', metric_type))
             for pid in processes:
                 worker_qout = processes[pid][1]
                 metric = worker_qout.get()
                 proc_metrics[pid] = metric
             # order processes by metric
-            proc_ranks = order_processes(proc_metrics, metric_type)
+            proc_ranks, best_metrics = order_processes(tracing, proc_metrics, metric_type)
             # cull
             culled_proc_ranks = cull(proc_ranks, pars['ga_reconstructions'][g])
             # remove culled processes from list (in the future we may reuse them)
             for i in range(len(culled_proc_ranks), len(proc_ranks)):
                 pid = proc_ranks[i][0]
                 worker_qin = processes[pid][0]
                 worker_qin.put('done')
                 processes.pop(pid)
-            # save results, we may modify it later to save only some
-            gen_save_dir = save_dir + '/g_' + str(g)
-            prev_dirs = {}
-            for i in range(len(culled_proc_ranks)):
-                pid = culled_proc_ranks[i][0]
+
+            # compare current alpha and previous. If previous is better, set it as alpha.
+            if (g == 0
+                    or
+                    best_metrics[metric_type] >= alpha_metrics[metric_type] and
+                    (metric_type == 'summed_phase' or metric_type == 'area')
+                    or
+                    best_metrics[metric_type] < alpha_metrics[metric_type] and
+                    (metric_type == 'chi' or metric_type == 'sharpness')):
+                pid = culled_proc_ranks[0][0]
                 worker_qin = processes[pid][0]
-                worker_qin.put(('save_res', gen_save_dir + '/' + str(i)))
-                prev_dirs[pid] = gen_save_dir + '/' + str(i)
-            for pid in processes:
+                worker_qin.put(('save_res', alpha_dir, True))
                 worker_qout = processes[pid][1]
                 ret = worker_qout.get()
+                alpha_metrics = best_metrics
+
+            # save results, we may modify it later to save only some
+            gen_save_dir = save_dir + '/g_' + str(g)
+            if g == pars['ga_generations'] -1:
+                for i in range(len(culled_proc_ranks)):
+                    pid = culled_proc_ranks[i][0]
+                    worker_qin = processes[pid][0]
+                    worker_qin.put(('save_res', gen_save_dir + '/' + str(i)))
+                for pid in processes:
+                    worker_qout = processes[pid][1]
+                    ret = worker_qout.get()
             if len(processes) == 0:
                 break
         for pid in processes:
             worker_qin = processes[pid][0]
             worker_qin.put('done')
     else:   # not fast GA
-        report_tracing = []
-        rec = multi
-        prev_dirs = []
-        if 'init_guess' not in pars:
-            pars['init_guess'] = 'random'
-        if pars['init_guess'] == 'continue':
-            continue_dir = pars['continue_dir']
-            for sub in os.listdir(continue_dir):
-                image, support, coh = ut.read_results(continue_dir + '/' + sub + '/')
-                if image is not None:
-                    prev_dirs.append(continue_dir + '/' + sub)
-                    report_tracing.append([continue_dir + '/' + sub])
-            if len(prev_dirs) < reconstructions:
-                for i in range(reconstructions - len(prev_dirs)):
-                    report_tracing.append(['random' + str(i)])
-                prev_dirs = prev_dirs + (reconstructions - len(prev_dirs)) * [None]
-        elif pars['init_guess'] == 'AI_guess':
-            import cohere_core.controller.AI_guess as ai
-            
-            report_tracing.append(['AI_guess'])
-            for i in range(reconstructions - 1):
-                report_tracing.append(['random' + str(i)])
-            ai_dir = ai.start_AI(pars, datafile, dir)
-            if ai_dir is None:
-                return
-            prev_dirs = [ai_dir] + (reconstructions - 1) * [None]
-        else:
-            for i in range(reconstructions):
-                prev_dirs.append(None)
-                report_tracing.append(['random' + str(i)])
-
         q = Queue()
-        # create alpha dir and placeholder for the alpha's metrics
-        alpha_dir = save_dir + '/alpha'
-        if not os.path.isdir(save_dir):
-            os.mkdir(save_dir)
-        if not os.path.isdir(alpha_dir):
-            os.mkdir(alpha_dir)
-        alpha_metrics = None
-
-        for g in range(generations):
+        prev_dirs = tracing.init_dirs
+        tracing.set_map({i:i for i in range(len(prev_dirs))})
+        rec = multi
+        for g in range(pars['ga_generations']):
             # delete previous-previous generation
             if g > 1:
                 shutil.rmtree(save_dir + '/g_' + str(g-2))
             print ('starting generation', g)
             gen_save_dir = save_dir + '/g_' + str(g)
             metric_type = pars['ga_metrics'][g]
             reconstructions = len(prev_dirs)
@@ -505,15 +553,15 @@
                 eval = r[0]
                 if eval is not None:
                     evals.append(eval)
                     temp_dirs.append(r[1])
 
             # results are saved in a list of directories - save_dir
             # it will be ranked, and moved to temporary ranked directories
-            current_dirs, report_tracing, best_metrics = order_dirs(report_tracing, temp_dirs, evals, metric_type, first_gen=(g==0))
+            current_dirs, best_metrics = order_dirs(tracing, temp_dirs, evals, metric_type)
             reconstructions = pars['ga_reconstructions'][g]
             current_dirs = cull(current_dirs, reconstructions)
             prev_dirs = current_dirs
 
             # compare current alpha and previous. If previous is better, set it as alpha.
             # no need toset alpha  for last generation
             if (g == 0
@@ -521,24 +569,13 @@
                     best_metrics[metric_type] >= alpha_metrics[metric_type] and
                     (metric_type == 'summed_phase' or metric_type == 'area')
                     or
                     best_metrics[metric_type] < alpha_metrics[metric_type] and
                     (metric_type == 'chi' or metric_type == 'sharpness')):
                 shutil.copyfile(current_dirs[0] + '/image.npy', alpha_dir + '/image.npy')
                 alpha_metrics = best_metrics
-
         # remove the previous gen
-        shutil.rmtree(save_dir + '/g_' + str(generations - 2))
-        # the report_tracing hold the ranking info. print it to a file
-        report_tracing.pop()
-        
-        try:
-            report_str = pretty_format_results(report_tracing)
-        except Exception as e:
-            print(f'WARNING: Report formatting failed due to {type(e)}: {e}! Falling back to raw formatting.')
-            report_str = '\n'.join([str(l) for l in report_tracing])
+        shutil.rmtree(save_dir + '/g_' + str(pars['ga_generations'] - 2))
 
-        with open(save_dir + '/ranks.txt', 'w+') as rank_file:
-            rank_file.write(report_str)
-            rank_file.flush()
+    tracing.save(save_dir)
 
-    print('done gen')
+    print('done gen')
```

### Comparing `cohere_core-3.2/cohere_core/data/alien_tools.py` & `cohere_core-4.0b0/cohere_core/data/alien_tools.py`

 * *Files identical despite different names*

### Comparing `cohere_core-3.2/cohere_core/data/standard_preprocess.py` & `cohere_core-4.0b0/cohere_core/data/standard_preprocess.py`

 * *Files identical despite different names*

### Comparing `cohere_core-3.2/cohere_core/lib/aflib.py` & `cohere_core-4.0b0/cohere_core/lib/aflib.py`

 * *Files identical despite different names*

### Comparing `cohere_core-3.2/cohere_core/lib/cplib.py` & `cohere_core-4.0b0/cohere_core/lib/cplib.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from cohere_core.lib.cohlib import cohlib
 import cupy as cp
 import numpy as np
 import cupyx.scipy.ndimage
+import cupyx.scipy.signal
 
 class cplib(cohlib):
     def array(obj):
         return cp.array(obj)
 
     def dot(arr1, arr2):
         return cp.dot(arr1, arr2)
 
     def set_device(dev_id):
-        cp.cuda.Device(dev_id).use()
+        if dev_id != -1:
+            cp.cuda.Device(dev_id).use()
 
     def set_backend(proc):
         pass
 
     def to_numpy(arr):
         return cp.asnumpy(arr)
 
@@ -50,26 +52,27 @@
 
     def fftshift(arr):
         return cp.fft.fftshift(arr)
 
     def ifftshift(arr):
         return cp.fft.ifftshift(arr)
 
-    def shift(arr, sft):
+    def shift(arr, sft, axis=None):
         sft = [int(s) for s in sft]
-        return cp.roll(arr, sft)
+        return cp.roll(arr, sft, axis=axis)
 
     def fft(arr):
         return cp.fft.fftn(arr, norm='forward')
 
     def ifft(arr):
         return cp.fft.ifftn(arr, norm='forward')
 
     def fftconvolve(arr1, arr2):
         return cupyx.scipy.ndimage.convolve(arr1, arr2)
+        # return cupyx.scipy.signal.aoconvolve(arr1, arr2, mode='same')
 
     def where(cond, x, y):
         return cp.where(cond, x, y)
 
     def dims(arr):
         # get array dimensions
         return arr.shape
@@ -158,7 +161,28 @@
         return cp.meshgrid(*xi)
 
     def exp(arr):
         return cp.exp(arr)
 
     def conj(arr):
         return cp.conj(arr)
+
+    def cos(arr):
+        return cp.cos(arr)
+
+    def linspace(start, stop, steps):
+        return cp.linspace(start, stop, steps)
+
+    def diff(arr, axis=None, prepend=0):
+        return cp.diff(arr, axis=axis, prepend=prepend)
+
+    def array_equal(arr1, arr2):
+        return cp.array_equal(arr1, arr2)
+
+    def cos(arr):
+        return cp.cos(arr)
+
+    def linspace(start, stop, num):
+        return cp.linspace(start, stop, num)
+
+    def clip(arr, min, max=None):
+        return cp.clip(arr, min, max)
```

### Comparing `cohere_core-3.2/cohere_core/lib/nplib.py` & `cohere_core-4.0b0/cohere_core/lib/nplib.py`

 * *Files 24% similar despite different names*

```diff
@@ -169,8 +169,26 @@
 
     def exp(arr):
         return np.exp(arr)
 
     def conj(arr):
         return np.conj(arr)
 
+    def array_equal(arr1, arr2):
+        return np.array_equal(arr1, arr2)
         # print(nplib.real(nplib.fft(nplib.gaussian((3,4,5),(3.0,4.0,5.0)))))
+
+    def cos(arr):
+        return np.cos(arr)
+
+    def linspace(start, stop, num):
+        return np.linspace(start, stop, num)
+
+    def clip(arr, min, max=None):
+        return np.clip(arr, min, max)
+
+# a11 = np.array([0.1, 0.2, 0.3, 1.0, 1.2, 1.3])
+# a12 = np.array([10.1, 10.2, 10.3, 11.0])
+# print(np.convolve(a11,a12, mode='same'))
+# from scipy.signal import convolve, fftconvolve
+# print(convolve(a11,a12, mode='same'))
+# print(fftconvolve(a11,a12, mode='same'))
```

### Comparing `cohere_core-3.2/cohere_core/utilities/config_errors_dict.py` & `cohere_core-4.0b0/cohere_core/utilities/config_errors_dict.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,50 +15,38 @@
                         'Parsing error, check parenthesis,quotation syntax'],
                 'Workingdir':['working_dir parameter should be a string',
                               'missing mandatory working_dir parameter'],
                 'ExperimentID':['experiment_id parameter should be string',
                                 'missing mandatory experiment_id parameter'],
                 'Scan':['scan parameter should be a string',
                         'scan parameter parsing error'],
-                'Specfile':['specfile parameter should be string',
-                            'specfile parameter parsing error']}
+                'Separatescans':['separate_scans parameter should be True or False'],
+                'Separatescanranges':['separate_scan_ranges parameter should be True or False'],
+                'Multipeak': ['multipeak parameter should be True or False']
+                }
 config_prep_error = {'File':['No configuration file',
                              'cannot read configuration file',
                              'Parsing error, check parenthesis,quotation syntax'],
                      'Roi':['roi parameter should be a list of int'],
                      'Datadir':['data_dir parameter should be string',
                                 'missing mandatory parameter data_dir'],
                      'Darkfield':['darkfield_filename parameter should be string',
                                   'darkfield_filename parameter parsing error'],
                      'Whitefield':['whitefield_filename parameter should be string',
                                    'whitefield_filename parameter parsing error'],
                      'Excludescans':['exclude scans should be a list'],
                      'MinFiles':['min_files should be int',
-                                 'min_files parameter parsing error'],
-                     'Separatescans':['separate_scans parameter should be True or False'],
-                     'Separatescanranges':['separate_scan_ranges parameter should be True or False']}
+                                 'min_files parameter parsing error']}
 config_disp_error = {'File':['No configuration file',
                              'Cannot read configuration file',
                              'Parsing error, check parenthesis,quotation syntax'],
                      'Resultsdir':['results_dir parameter should be string'],
-                     'Diffractometer':['diffractometer parameter should be string'],
-                     'Detector':['detector parameter should be string'],
                      'Crop':['crop should be list',
                              'crop should be a list of int or float'],
-                     'Rampups':['rampups should be int'],
-                     'Energy':['energy should be float',
-                               'energy parameter parsing error'],
-                     'Delta':['delta should be float',
-                              'delta parameter parsing error'],
-                     'Gamma':['gamma should be float',
-                              'gamma parameter parsing error'],
-                     'Detdist':['detdist should be float',
-                                'detdist parameter parsing error'],
-                     'Dth':['dth should be float',
-                            'dth parameter parsing error']}
+                     'Rampups':['rampups should be int']}
 config_data_error = {'File':['No configuration file',
                              'Cannot read configuration file',
                              'Parsing error, check parenthesis,quotation syntax'],
                      'Datadir':['data_dir parameter should be string',
                                 'data_dir parameter parsing error'],
                      'Adjustdimensions':['adjust_dimensions should be a list of int'],
                      'Centershift':['center_shift should be a list of int'],
@@ -109,56 +97,81 @@
                                          'missing mandatory algorithm_sequence parameter'],
                     'Hiobeta':['hio_beta parameter should be float'],
                     'Initialsupportarea':['initial_support_area should be list',
                                           'initial_support_area should be a list of int or float'],
                     'Generations':['ga_generations parameter should be int',
                                    'when running GA "reconstructions" parameter should be configured and greater than 1'],
                     'Gametrics':['ga_metrics is not a list',
-                                 'ga_metrics list can include only following strings: "chi", "sharpness", "summed_phase", "area"'],
+                                 'warning: ga_metrics list can include only following strings: "chi", "sharpness", "summed_phase", "area"'],
                     'Gabreedmodes':['ga_breed_mode is not a list',
-                                    'ga_breed_modes list can include only following strings: “none”, “sqrt_ab”, “dsqrt”,“pixel_switch”, “b_pa”, “2ab_a_b”, “2a_b_pa”,'
+                                    'warning: ga_breed_modes list can include only following strings: “none”, “sqrt_ab”, “pixel_switch”, “b_pa”, “2ab_a_b”, “2a_b_pa”,'
                                     ' “sqrt_ab_pa”, “sqrt_ab_pa_recip”, “sqrt_ab_recip”,“max_ab”, “max_ab_pa”, '
                                     '“min_ab_pa”, “avg_ab”, “avg_ab_pa"'],
                     'Gacullings':['ga_cullings parameter should be a ist of int',
                                   'sum of all cullings should be smaller than number of reconstructions'],
-                    'Gashrinkwrapthresholds':['ga_shrink_wrap_thresholds parameter should be a list of floats'],
-                    'Gashrinkwrapgausssigmas':['ga_shrink_wrap_gauss_sigmas parameter should be a list of floats'],
+                    'Gashrinkwrapthresholds':['ga_sw_thresholds parameter should be a list of floats'],
+                    'Gashrinkwrapgausssigmas':['ga_sw_gauss_sigmas parameter should be a list of floats'],
                     'Galowpassfiltersigmas':['List Float Error',
-                                             'ga_shrink_wrap_gauss_sigmas parameter parsing error'],
+                                             'ga_sw_gauss_sigmas parameter parsing error'],
                     'Gagenpcstart':['ga_gen_pc_start parameter should be int',
                                     'ga_gen_pc_start parameter parsing error'],
                     'Twintrigger':['Trigger should be a list of int'],
                     'Twinhalves':['twin_halves should be a list of int'],
-                    'Shrinkwraptrigger':['Trigger should be a list of int'],
-                    'Shrinkwraptype':['shrink_wrap_type parameter should be string',
-                                      'supporting shrink_wrap_type "GAUSS"'],
-                    'Shrinkwrapthreshold':['shrink_wrap_threshold should be float',
-                                           'shrink_wrap_threshold parameter parsing error'],
-                    'Shrinkwrapgausssigma':['shrink_wrap_gauss_sigma should be float',
-                                            'shrink_wrap_gauss_sigma parameter parsing error'],
-                    'Phasesupporttrigger':['Trigger should be a list of int'],
+                    'Shrinkwraptrigger':['Trigger should be a list of int',
+                                         'Each sub-trigger should be a list of int if multiple shrink wraps'],
+                    'Shrinkwraptype':['sw_type parameter should be string',
+                                      'supporting sw_type "GAUSS"'],
+                    'Shrinkwrapthreshold':['sw_threshold should be float',
+                                           'sw_threshold should be a list of floats if multiple shrink wraps'],
+                    'Shrinkwrapgausssigma':['sw_gauss_sigma should be float',
+                                            'sw_gauss_sigma should be a list of floats if multiple shrink wraps'],
+                    'Phasesupporttrigger':['Trigger should be a list of int',
+                                           'Each sub-trigger should be a list of int if multiple phase modulus'],
                     'Phmphasemin':['phm_phase_min should be float',
-                                   'phm_phase_min parameter parsing error'],
+                                   'phm_phase_min should be a list of floats if multiple phase modulus'],
                     'Phmphasemax':['phm_phase_max should be float',
-                                   'phm_phase_max parameter parsing error'],
+                                   'phm_phase_max should be a list of floats if multiple phase modulus'],
                     'Pcinterval':['pc_interval should be int'],
                     'Pctype':['pc_type parameter should be string',
                               'pc_type parameter can be configured "LUCY"',
                               'pc_type parameter parsing error'],
                     'Pclucyiterations':['pc_LUCY_iterations should be int',
                                        'pc_LUCY_iterations parameter parsing error'],
                     'Pcnormalize':['pc_normalize parameter should be True or False',
                                    'pc_normalize parameter parsing error'],
                     'Pclucykernel':['pc_LUCY_kernel parameter should be a list of int',
                                     'pc_LUCY_kernel parameter must be configured when partial coherence feature in active'],
-                    'Resolutiontrigger':['Trigger should be a list of int'],
-                    'Lowpassfilterswsigmarange':['lowpass_filter_sw_sigma_range parameter should be list of flots'],
-                    'Lowpassfilterrange':['lowpass_filter_range parameter should be list of flots'],
+                    'lpftrigger':['Trigger should be a list of int',
+                                    'Each sub-trigger should be a list of int if multiple lowpass filters'],
+                    'Lowpassfilterswthreshold':['lpf_sw_threshold parameter should be flot',
+                                                'lpf_sw_threshold should be a list of floats if multiple lowpass filters'],
+                    'Lowpassfilterrange':['lowpass_filter_range parameter should be list of flots',
+                                          'lowpass_filter_range should be a list of int for each lowpass filter if multiple lowpass filters'
+                                          'missing lowpass_filter_range parameter'],
                     'Averagetrigger':['Trigger should be a list of int'],
                     'Progresstrigger':['Trigger should be a list of int'],
                     }
 
+config_instr_error = { 'Diffractometer':['missing mandatory diffractometer parameter',
+                                         'diffractometer parameter should be string'],
+                       'Specfile': ['missing mandatory specfile parameter',
+                                    'specfile parameter should be string',
+                                    'specfile parameter parsing error'],
+                       'Detector':['detector parameter should be string'],
+                       'Energy':['energy should be float',
+                                 'energy parameter parsing error'],
+                       'Delta':['delta should be float',
+                                'delta parameter parsing error'],
+                       'Gamma':['gamma should be float',
+                                'gamma parameter parsing error'],
+                       'Detdist':['detdist should be float',
+                                  'detdist parameter parsing error'],
+                       'Dth':['dth should be float',
+                              'dth parameter parsing error']
+                    }
+
 config_map_names = {'config_error_map_file':config_error,
                     'config_prep_error_map_file':config_prep_error,
                     'config_disp_error_map_file':config_disp_error,
                     'config_data_error_map_file':config_data_error,
-                    'config_rec_error_map_file':config_rec_error}
+                    'config_rec_error_map_file':config_rec_error,
+                    'config_instr_error_map_file':config_instr_error}
```

### Comparing `cohere_core-3.2/cohere_core/utilities/config_verifier.py` & `cohere_core-4.0b0/cohere_core/utilities/config_verifier.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 ===========================
 
 Verification of configuration parameters.
 """
 
 import os
 from cohere_core.utilities.config_errors_dict import *
+from cohere_core.controller.op_flow import algs
 
 __author__ = "Barbara Frosik, Dave Cyl"
 __copyright__ = "Copyright (c) 2016, UChicago Argonne, LLC."
 __docformat__ = 'restructuredtext en'
 __all__ = ['verify']
            
 
@@ -143,14 +144,41 @@
         scan = config_map['scan']
         if type(scan) != str:
             config_error = 0
             error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
             print(error_message)
             return (error_message)
 
+    config_parameter = 'Separatescans'
+    if 'separate_scans' in config_map:
+        separate_scans = config_map['separate_scans']
+        if type(separate_scans) != bool:
+            config_error = 0
+            error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
+            print(error_message)
+            return (error_message)
+
+    config_parameter = 'Separatescanranges'
+    if 'separate_scan_ranges' in config_map:
+        separate_scan_ranges = config_map['separate_scan_ranges']
+        if type(separate_scan_ranges) != bool:
+            config_error = 0
+            error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
+            print(error_message)
+            return (error_message)
+
+    config_parameter = 'Multipeak'
+    if 'multipeak' in config_map:
+        separate_scans = config_map['multipeak']
+        if type(separate_scans) != bool:
+            config_error = 0
+            error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
+            print(error_message)
+            return (error_message)
+
     return ("")
 
 
 def ver_config_rec(config_map):
     """
     This function verifies experiment config_rec file
 
@@ -162,14 +190,65 @@
     Returns
     -------
     error_message : str
         message describing parameter error or empty string if all parameters are verified
     """
     import string
 
+    def get_no_iter(s):
+        seq = []
+        def parse_entry(ent):
+            r_e = ent.split('*')
+            # if r_e[1] not in algs:
+            #     return r_e[1] + ' is not a valid entry in algorithm_sequence parameter'
+            seq.append([int(r_e[0]), r_e[1]])
+            return ''
+
+        s = s.replace(' ','')
+        entries = s.split('+')
+        i = 0
+        while i < len(entries):
+            entry = entries[i]
+            if '(' in entry:
+                group = []
+                rep_entry = entry.split('(')
+                repeat = int(rep_entry[0][:-1])
+                group.append(rep_entry[1])
+                i += 1
+                group_entry = entries[i]
+                while ')' not in group_entry:
+                    group.append(group_entry)
+                    i += 1
+                    group_entry = entries[i]
+                group.append(group_entry[:-1])
+                for _ in range(repeat):
+                    for group_entry in group:
+                        msg = parse_entry(group_entry)
+                        if len(msg) > 0:
+                            return msg, 0
+                i += 1
+            else:
+                msg = parse_entry(entry)
+                if len(msg) > 0:
+                    return msg, 0
+                i += 1
+        return '', sum([e[0] for e in seq])
+
+
+    def verify_trigger(trigger, no_iter):
+        if len(trigger) == 0:
+            return ('empty trigger ' + str(trigger))
+        elif trigger[0] >= no_iter:
+            return ('trigger start ' + str(trigger[0]) + ' exceeds number of iterations ' + str(no_iter))
+        if len(trigger) == 3:
+            if trigger[2] >= no_iter:
+                return ('trigger end ' + str(trigger[2]) + ' exceeds number of iterations ' + str(no_iter))
+        return ''
+
+
     config_map_file = 'config_rec_error_map_file'
     fname = 'config_rec'
 
     config_parameter = 'Datadir'
     if 'data_dir' in config_map:
         data_dir = config_map['data_dir']
         if type(data_dir) != str:
@@ -259,15 +338,15 @@
         algorithm_sequence = config_map['algorithm_sequence']
         if type(algorithm_sequence) != str:
             config_error = 0
             error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
             print (config_error)
             return (error_message)
         # check for supported characters
-        alg_seq_chars = list(string.ascii_lowercase) + list(string.ascii_uppercase) + list(string.digits) + ['*', '+', '(', ')', ' ']
+        alg_seq_chars = list(string.ascii_lowercase) + list(string.ascii_uppercase) + list(string.digits) + ['.','*', '+', '(', ')', ' ']
         if 0 in [c in alg_seq_chars for c in algorithm_sequence]:
             config_error = 1
             error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
             print(config_error)
             return (error_message)
         # check brackets, nested are not allowed
         br_count = 0
@@ -281,14 +360,23 @@
                 if br_count < 0:
                     break
         if br_count != 0:
             config_error = 2
             error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
             print(config_error)
             return (error_message)
+        # calculate number of iterations
+        try:
+            msg, iter_no = get_no_iter(algorithm_sequence)
+            if len(msg) > 0:
+                print(msg)
+                return msg
+        except Exception as e:
+            print('check algorithm_sequence')
+            return ('check algorithm_sequence')
     else:
         config_error = 3
         error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
         print (error_message)
         return (error_message)
 
     config_parameter = 'Hiobeta'
@@ -343,32 +431,32 @@
                 return (error_message)
             metrics_options = ['chi', 'sharpness', 'summed_phase', 'area']
             for metric in ga_metrics:
                 if metric not in metrics_options:
                     config_error = 1
                     error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
                     print (error_message)
-                    return (error_message)
+                    return ('') 
 
         config_parameter = 'Gabreedmodes'
         if 'ga_breed_modes' in config_map:
             ga_breed_modes = config_map['ga_breed_modes']
             if not issubclass(type(ga_breed_modes), list):
                 config_error = 0
                 error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
                 print (error_message)
                 return (error_message)
-            breed_options = ['none', 'sqrt_ab', 'dsqrt', 'pixel_switch', 'b_pa', '2ab_a_b', '2a_b_pa', 'sqrt_ab_pa',\
+            breed_options = ['none', 'sqrt_ab', 'pixel_switch', 'b_pa', '2ab_a_b', '2a_b_pa', 'sqrt_ab_pa',\
 'sqrt_ab_pa_recip', 'sqrt_ab_recip', 'max_ab', 'max_ab_pa', 'min_ab_pa', 'avg_ab', 'avg_ab_pa']
             for breed in ga_breed_modes:
                 if breed not in breed_options:
                     config_error = 1
                     error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
                     print (error_message)
-                    return (error_message)
+                    return ('')
 
         config_parameter = 'Gacullings'
         if 'ga_cullings' in config_map:
             ga_cullings = config_map['ga_cullings']
             if not ver_list_int('ga_cullings', ga_cullings):
                 config_error = 0
                 error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
@@ -377,35 +465,35 @@
             if sum(ga_cullings) >= reconstructions:
                 config_error = 1
                 error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
                 print(error_message)
                 return (error_message)
 
         config_parameter = 'Gashrinkwrapthresholds'
-        if 'ga_shrink_wrap_thresholds' in config_map:
-            ga_shrink_wrap_thresholds = config_map['ga_shrink_wrap_thresholds']
-            if not ver_list_float('ga_shrink_wrap_thresholds', ga_shrink_wrap_thresholds):
+        if 'ga_sw_thresholds' in config_map:
+            ga_sw_thresholds = config_map['ga_sw_thresholds']
+            if not ver_list_float('ga_sw_thresholds', ga_sw_thresholds):
                 config_error = 0
                 error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
                 print(error_message)
                 return (error_message)
 
         config_parameter = 'Gashrinkwrapgausssigmas'
-        if 'ga_shrink_wrap_gauss_sigmas' in config_map:
-            ga_shrink_wrap_gauss_sigmas = config_map['ga_shrink_wrap_gauss_sigmas']
-            if not ver_list_float('ga_shrink_wrap_gauss_sigmas', ga_shrink_wrap_gauss_sigmas):
+        if 'ga_sw_gauss_sigmas' in config_map:
+            ga_sw_gauss_sigmas = config_map['ga_sw_gauss_sigmas']
+            if not ver_list_float('ga_sw_gauss_sigmas', ga_sw_gauss_sigmas):
                 config_error = 0
                 error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
                 print(error_message)
                 return (error_message)
 
         config_parameter = 'Galowpassfiltersigmas'
-        if 'ga_lowpass_filter_sigmas' in config_map:
-            ga_lowpass_filter_sigmas = config_map['ga_lowpass_filter_sigmas']
-            if not ver_list_float('ga_lowpass_filter_sigmas', ga_lowpass_filter_sigmas):
+        if 'ga_lpf_sigmas' in config_map:
+            ga_lpf_sigmas = config_map['ga_lpf_sigmas']
+            if not ver_list_float('ga_lpf_sigmas', ga_lpf_sigmas):
                 config_error = 0
                 error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
                 return (error_message)
 
         config_parameter = 'Gagenpcstart'
         if 'ga_gen_pc_start' in config_map:
             ga_gen_pc_start = config_map['ga_gen_pc_start']
@@ -414,14 +502,17 @@
                 error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
                 print(error_message)
                 return (error_message)
 
     config_parameter = 'Twintrigger'
     if 'twin_trigger' in config_map:
         twin_trigger = config_map['twin_trigger']
+        m = verify_trigger(twin_trigger, iter_no)
+        if len(m) > 0:
+            return(m)
         if not ver_list_int('twin_trigger', twin_trigger):
             config_error = 0
             error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
             print(error_message)
             return (error_message)
 
         config_parameter = 'Twinhalves'
@@ -431,86 +522,141 @@
                 config_error = 0
                 error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
                 print(error_message)
                 return (error_message)
 
     config_parameter = 'Shrinkwraptrigger'
     if 'shrink_wrap_trigger' in config_map:
-        if not ver_list_int('shrink_wrap_trigger', config_map['shrink_wrap_trigger']):
-            config_error = 0
-            error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
-            print(error_message)
-            return (error_message)
-
-        config_parameter = 'Shrinkwraptype'
-        if 'shrink_wrap_type' in config_map:
-            shrink_wrap_type = config_map['shrink_wrap_type']
-            if type(shrink_wrap_type) != str:
-                config_error = 0
-                error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
-                print (error_message)
-                return (error_message)
-            if shrink_wrap_type != "GAUSS":
-                config_error = 1
-                error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
-                print (error_message)
-                return (error_message)
-
-        config_parameter = 'Shrinkwrapthreshold'
-        if 'shrink_wrap_threshold' in config_map:
-            shrink_wrap_threshold = config_map['shrink_wrap_threshold']
-            if type(shrink_wrap_threshold) != float:
+        if '.SW' not in config_map['algorithm_sequence']:
+            m = verify_trigger(config_map['shrink_wrap_trigger'], iter_no)
+            if len(m) > 0:
+                return(m)
+            if not ver_list_int('shrink_wrap_trigger', config_map['shrink_wrap_trigger']):
                 config_error = 0
                 error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
                 print(error_message)
                 return (error_message)
 
-        config_parameter = 'Shrinkwrapgausssigma'
-        if 'shrink_wrap_gauss_sigma' in config_map:
-            shrink_wrap_gauss_sigma = config_map['shrink_wrap_gauss_sigma']
-            if type(shrink_wrap_gauss_sigma) != float and type(shrink_wrap_gauss_sigma) != int:
-                config_error = 0
-                error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
-                print(error_message)
-                return (error_message)
+            config_parameter = 'Shrinkwraptype'
+            if 'shrink_wrap_type' in config_map:
+                shrink_wrap_type = config_map['shrink_wrap_type']
+                if type(shrink_wrap_type) != str:
+                    config_error = 0
+                    error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
+                    print (error_message)
+                    return (error_message)
+                if shrink_wrap_type != "GAUSS":
+                    config_error = 1
+                    error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
+                    print (error_message)
+                    return (error_message)
 
-    config_parameter = 'Phasesupporttrigger'
-    if 'phase_support_trigger' in config_map:
-        if not ver_list_int('phase_support_trigger', config_map['phase_support_trigger']):
-            config_error = 0
-            error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
-            print(error_message)
-            return (error_message)
+            config_parameter = 'Shrinkwrapthreshold'
+            if 'shrink_wrap_threshold' in config_map:
+                shrink_wrap_threshold = config_map['shrink_wrap_threshold']
+                if type(shrink_wrap_threshold) != float:
+                    config_error = 0
+                    error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
+                    print(error_message)
+                    return (error_message)
 
-        config_parameter = 'Phmphasemin'
-        if 'phm_phase_min' in config_map:
-            phm_phase_min = config_map['phm_phase_min']
-            if type(phm_phase_min) != float:
-                config_error = 0
-                error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
-                print(error_message)
-                return (error_message)
+            config_parameter = 'Shrinkwrapgausssigma'
+            if 'shrink_wrap_gauss_sigma' in config_map:
+                shrink_wrap_gauss_sigma = config_map['shrink_wrap_gauss_sigma']
+                if type(shrink_wrap_gauss_sigma) != float and type(shrink_wrap_gauss_sigma) != int:
+                    config_error = 0
+                    error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
+                    print(error_message)
+                    return (error_message)
+        else:
+            for t in config_map['shrink_wrap_trigger']:
+                if not ver_list_int('shrink_wrap_trigger', t):
+                    config_error = 1
+                    error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
+                    print(error_message)
+                    return (error_message)
+            config_parameter = 'Shrinkwrapthreshold'
+            if 'shrink_wrap_threshold' in config_map:
+                if not ver_list_float('shrink_wrap_threshold', config_map['shrink_wrap_threshold']):
+                    config_error = 1
+                    error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
+                    print(error_message)
+                    return (error_message)
+
+            config_parameter = 'Shrinkwrapgausssigma'
+            if 'shrink_wrap_gauss_sigma' in config_map:
+                if not ver_list_float('shrink_wrap_gauss_sigma', config_map['shrink_wrap_gauss_sigma']):
+                    config_error = 1
+                    error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
+                    print(error_message)
+                    return (error_message)
 
-        config_parameter = 'Phmphasemax'
-        if 'phm_phase_max' in config_map:
-            phm_phase_max = config_map['phm_phase_max']
-            if type(phm_phase_max) != float:
+    config_parameter = 'Phasesupporttrigger'
+    if 'phm_trigger' in config_map:
+        if '.PHM' not in config_map['algorithm_sequence']:
+            m = verify_trigger(config_map['phm_trigger'], iter_no)
+            print(m)
+            if len(m) > 0:
+                return(m)
+            if not ver_list_int('phm_trigger', config_map['phm_trigger']):
                 config_error = 0
                 error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
                 print(error_message)
                 return (error_message)
 
+            config_parameter = 'Phmphasemin'
+            if 'phm_phase_min' in config_map:
+                phm_phase_min = config_map['phm_phase_min']
+                if type(phm_phase_min) != float:
+                    config_error = 0
+                    error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
+                    print(error_message)
+                    return (error_message)
+
+            config_parameter = 'Phmphasemax'
+            if 'phm_phase_max' in config_map:
+                phm_phase_max = config_map['phm_phase_max']
+                if type(phm_phase_max) != float:
+                    config_error = 0
+                    error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
+                    print(error_message)
+                    return (error_message)
+        else:
+            for t in config_map['phm_trigger']:
+                if not ver_list_int('phm_trigger', t):
+                    config_error = 1
+                    error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
+                    print(error_message)
+                    return (error_message)
+            config_parameter = 'Phmphasemin'
+            if 'phm_phase_min' in config_map:
+                if not ver_list_float('phm_phase_min', config_map['phm_phase_min']):
+                    config_error = 1
+                    error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
+                    print(error_message)
+                    return (error_message)
+
+            config_parameter = 'Phmphasemax'
+            if 'phm_phase_max' in config_map:
+                if not ver_list_float('phm_phase_max', config_map['phm_phase_max']):
+                    config_error = 1
+                    error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
+                    print(error_message)
+                    return (error_message)
+
     config_parameter = 'Pcinterval'
     if 'pc_interval' in config_map:
         pc_interval = config_map['pc_interval']
         if type(pc_interval) != int:
             config_error = 0
             error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
             print(error_message)
             return (error_message)
+        if pc_interval >= iter_no:
+            return('pc_interval', pc_interval, 'exceeds number of iterations', iter_no)
 
         config_parameter = 'Pctype'
         if 'pc_type' in config_map:
             pc_type = config_map['pc_type']
             if type(pc_type) != str:
                 config_error = 0
                 error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
@@ -551,49 +697,94 @@
         else:
             config_error = 1
             error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
             print(error_message)
             return (error_message)
 
     config_parameter = 'Resolutiontrigger'
-    if 'resolution_trigger' in config_map:
-        if not ver_list_int('resolution_trigger', config_map['resolution_trigger']):
-            config_error = 0
-            error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
-            print(error_message)
-            return (error_message)
-
-        config_parameter = 'Lowpassfilterswsigmarange'
-        if 'lowpass_filter_sw_sigma_range' in config_map:
-            lowpass_filter_sw_sigma_range = config_map['lowpass_filter_sw_sigma_range']
-            if not ver_list_float('lowpass_filter_sw_sigma_range', lowpass_filter_sw_sigma_range):
+    if 'lowpass_filter_trigger' in config_map:
+        if '.LPF' not in config_map['algorithm_sequence']:
+            m = verify_trigger(config_map['lowpass_filter_trigger'], iter_no)
+            if len(m) > 0:
+                return(m)
+            if not ver_list_int('lowpass_filter_trigger', config_map['lowpass_filter_trigger']):
                 config_error = 0
                 error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
                 print(error_message)
                 return (error_message)
 
-        config_parameter = 'Lowpassfilterrange'
-        if 'lowpass_filter_range' in config_map:
-            lowpass_filter_range = config_map['lowpass_filter_range']
-            if not ver_list_float('lowpass_filter_range', lowpass_filter_range):
-                config_error = 0
+            config_parameter = 'Lowpassfilterswthreshold'
+            if 'lowpass_filter_sw_threshold' in config_map:
+                lowpass_filter_sw_threshold = config_map['lowpass_filter_sw_threshold']
+                if type(lowpass_filter_sw_threshold) != float:
+                    error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
+                    print(error_message)
+                    return (error_message)
+
+            config_parameter = 'Lowpassfilterrange'
+            if 'lowpass_filter_range' in config_map:
+                lowpass_filter_range = config_map['lowpass_filter_range']
+                if not ver_list_float('lowpass_filter_range', lowpass_filter_range):
+                    config_error = 0
+                    error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
+                    print(error_message)
+                    return (error_message)
+            else:
+                config_error = 2
+                error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
+                print(error_message)
+                return (error_message)
+        else:
+            for t in config_map['lowpass_filter_trigger']:
+                if not ver_list_int('lowpass_filter_trigger', t):
+                    config_error = 1
+                    error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
+                    print(error_message)
+                    return (error_message)
+
+            config_parameter = 'Lowpassfilterrange'
+            if 'lowpass_filter_range' in config_map:
+                for r in config_map['lowpass_filter_range']:
+                    if not ver_list_float('lowpass_filter_range', r):
+                        config_error = 1
+                        error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
+                        print(error_message)
+                        return (error_message)
+            else:
+                config_error = 2
                 error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
                 print(error_message)
                 return (error_message)
 
+            config_parameter = 'Lowpassfilterswthreshold'
+            if 'lowpass_filter_sw_threshold' in config_map:
+                lowpass_filter_sw_threshold = config_map['lowpass_filter_sw_threshold']
+                if not ver_list_float('lowpass_filter_sw_threshold', lowpass_filter_sw_threshold):
+                    config_error = 1
+                    error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
+                    print(error_message)
+                    return (error_message)
+
+
     config_parameter = 'Averagetrigger'
     if 'average_trigger' in config_map:
+        m = verify_trigger(config_map['average_trigger'], iter_no)
+        if len(m) > 0:
+            return(m)
         if not ver_list_int('average_trigger', config_map['average_trigger']):
             config_error = 0
             error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
             print(error_message)
             return (error_message)
 
     config_parameter = 'Progresstrigger'
     if 'progress_trigger' in config_map:
+        m = verify_trigger(config_map['progress_trigger'], iter_no)
+        if len(m) > 0:
+            return(m)
         if not ver_list_int('progress_trigger', config_map['progress_trigger']):
             config_error = 0
             error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
             print(error_message)
             return (error_message)
 
     # return empty string if verified
@@ -859,32 +1050,14 @@
     if 'exclude_scans' in config_map:
         if not ver_list_int('exclude_scans', config_map['exclude_scans']):
             config_error = 0
             error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
             print (error_message)
             return (error_message)
 
-    config_parameter = 'Separatescans'
-    if 'separate_scans' in config_map:
-        separate_scans = config_map['separate_scans']
-        if type(separate_scans) != bool:
-            config_error = 0
-            error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
-            print(error_message)
-            return (error_message)
-
-    config_parameter = 'Separatescanranges'
-    if 'separate_scan_ranges' in config_map:
-        separate_scan_ranges = config_map['separate_scan_ranges']
-        if type(separate_scan_ranges) != bool:
-            config_error = 0
-            error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
-            print(error_message)
-            return (error_message)
-
     return ("")
 
 
 def ver_config_disp(config_map):
     """
     This function verifies experiment config_disp file
 
@@ -996,14 +1169,141 @@
             error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
             print('dth should be float')
             return (error_message)
 
     return ("")
 
 
+
+def ver_config_instr(config_map):
+    """
+    This function verifies experiment config_disp file
+
+    Parameters
+    ----------
+    fname : str
+        configuration file name
+
+    Returns
+    -------
+    error_message : str
+        message describing parameter error or empty string if all parameters are verified
+    """
+    config_map_file = 'config_instr_error_map_file'
+    fname = 'config_instr'
+
+    config_parameter = 'Diffractometer'
+    if 'diffractometer' in config_map:
+        diffractometer = config_map['diffractometer']
+        if type(diffractometer) != str:
+            config_error = 1
+            error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
+            print('diffractometer parameter should be string')
+            return (error_message)
+    else:
+        config_error = 0
+        error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
+        print('missing mandatory diffractometer parameter')
+        return ''
+
+    config_parameter = 'Specfile'
+    if 'specfile' in config_map:
+        specfile = config_map['specfile']
+        if type(specfile) != str:
+            config_error = 1
+            error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
+            print('specfile parameter should be string')
+            return (error_message)
+    else:
+        config_error = 0
+        error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
+        print('missing mandatory specfile parameter')
+        return ''
+
+    config_parameter = 'Detector'
+    if 'detector' in config_map:
+        detector = config_map['detector']
+        if type(detector) != str:
+            config_error = 0
+            error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
+            print('detector parameter should be string')
+            return (error_message)
+
+    config_parameter = 'Crop'
+    if 'crop' in config_map:
+        crop = config_map['crop']
+        if not issubclass(type(crop), list):
+            config_error = 0
+            error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
+            print('crop should be list')
+            return (error_message)
+        for e in crop:
+            if type(e) != int and type(e) != float:
+                config_error = 1
+                error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
+                print('crop should be a list of int or float')
+                return (error_message)
+
+    config_parameter = 'Rampups'
+    if 'rampups' in config_map:
+        rampups = config_map['rampups']
+        if type(rampups) != int:
+            config_error = 0
+            error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
+            print('rampups should be float')
+            return (error_message)
+
+    config_parameter = 'Energy'
+    if 'energy' in config_map:
+        energy = config_map['energy']
+        if type(energy) != float:
+            config_error = 0
+            error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
+            print('energy should be float')
+            return (error_message)
+
+    config_parameter = 'Delta'
+    if 'delta' in config_map:
+        delta = config_map['delta']
+        if type(delta) != float:
+            config_error = 0
+            error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
+            print('delta should be float')
+            return (error_message)
+
+    config_parameter = 'Gamma'
+    if 'gamma' in config_map:
+        gamma = config_map['gamma']
+        if type(gamma) != float:
+            config_error = 0
+            error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
+            print('gamma should be float')
+            return (error_message)
+
+    config_parameter = 'Detdist'
+    if 'detdist' in config_map:
+        detdist = config_map['detdist']
+        if type(detdist) != float:
+            config_error = 0
+            error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
+            print('detdist should be float')
+            return (error_message)
+
+    config_parameter = 'Dth'
+    if 'dth' in config_map:
+        dth = config_map['dth']
+        if type(dth) != float:
+            config_error = 0
+            error_message = get_config_error_message(fname, config_map_file, config_parameter, config_error)
+            print('dth should be float')
+            return (error_message)
+
+    return ("")
+
+
 def verify(file_name, conf_map):
     """
     Verifies parameters.
 
     Parameters
     ----------
     file_name : str
@@ -1023,9 +1323,11 @@
         return ver_config_prep(conf_map)
     elif file_name == 'config_data':
         return ver_config_data(conf_map)
     elif file_name == 'config_rec':
         return ver_config_rec(conf_map)
     elif file_name == 'config_disp':
         return ver_config_disp(conf_map)
+    elif file_name == 'config_instr':
+        return ver_config_instr(conf_map)
     else:
         return ('verifier has no fumction to check config file named', file_name)
```

### Comparing `cohere_core-3.2/cohere_core/utilities/dvc_utils.py` & `cohere_core-4.0b0/cohere_core/utilities/dvc_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,13 @@
 import math
-import importlib
-import os
 
 
-def set_lib(dlib, is_af):
+def set_lib(dlib):
     global dvclib
-    global dvclib2
     dvclib = dlib
-    if is_af:
-        dvclib2 = importlib.import_module('cohere_core.lib.aflib').aflib2
-    else:
-        dvclib2 = dvclib
 
 
 def crop_center(arr, shape):
     dims = dvclib.dims(arr)
     principio = []
     finem = []
     for i in range(3):
@@ -272,25 +265,25 @@
     if nor < 0:
         nor = nr
     if noc < 0:
         noc = nc
 
     # Compute kernels and obtain DFT by matrix products
     yl = list(range(-int(math.floor(nc / 2)), nc - int(math.floor(nc / 2))))
-    y = dvclib2.ifftshift(dvclib.array(yl)) * (-2j * math.pi / (nc * usfac))
+    y = dvclib.ifftshift(dvclib.array(yl)) * (-2j * math.pi / (nc * usfac))
     xl = list(range(-coff, noc - coff))
     x = dvclib.array(xl)
     yt = dvclib.tile(y, (len(xl), 1))
     xt = dvclib.tile(x, (len(yl), 1))
-    kernc = dvclib2.exp(yt.T * xt)
+    kernc = dvclib.exp(yt.T * xt)
 
     yl = list(range(-roff, nor - roff))
     y = dvclib.array(yl)
     xl = list(range(-int(math.floor(nr / 2)), nr - int(math.floor(nr / 2))))
-    x = dvclib2.ifftshift(dvclib.array(xl))
+    x = dvclib.ifftshift(dvclib.array(xl))
     yt = dvclib.tile(y, (len(xl), 1))
     xt = dvclib.tile(x, (len(yl), 1))
     kernr = dvclib.exp(yt * xt.T * (-2j * math.pi / (nr * usfac)))
 
     # return as device array
     return dvclib.dot(dvclib.dot(kernr.T, arr), kernc)
 
@@ -317,19 +310,19 @@
     if usfac < 2:
         print('usfac less than 2 not supported')
         return
     # First upsample by a factor of 2 to obtain initial estimate
     # Embed Fourier data in a 2x larger array
     shape = ref_arr.shape
     large_shape = tuple(2 * x for x in ref_arr.shape)
-    c_c = pad_around(dvclib2.fftshift(ref_arr) * dvclib.conj(dvclib2.fftshift(arr)), large_shape, val=0j)
+    c_c = pad_around(dvclib.fftshift(ref_arr) * dvclib.conj(dvclib.fftshift(arr)), large_shape, val=0j)
 
     # Compute crosscorrelation and locate the peak
-    c_c = dvclib2.ifft(dvclib2.ifftshift(c_c))    #TODO will not work for aflib
-    max_coord = dvclib2.unravel_index(dvclib2.argmax(c_c), dvclib.dims(c_c))
+    c_c = dvclib.ifft(dvclib.ifftshift(c_c))    #TODO will not work for aflib
+    max_coord = dvclib.unravel_index(dvclib.argmax(c_c), dvclib.dims(c_c))
 
     if max_coord[0] > shape[0]:
         row_shift = max_coord[0] - large_shape[0]
     else:
         row_shift = max_coord[0]
     if max_coord[1] > shape[1]:
         col_shift = max_coord[1] - large_shape[1]
@@ -339,23 +332,23 @@
     row_shift = row_shift / 2
     col_shift = col_shift / 2
 
     # If upsampling > 2, then refine estimate with matrix multiply DFT
     if usfac > 2:
         # DFT computation
         # Initial shift estimate in upsampled grid
-        row_shift = dvclib2.round(row_shift * usfac) / usfac
-        col_shift = dvclib2.round(col_shift * usfac) / usfac
-        dftshift = dvclib2.fix(dvclib.ceil(usfac * 1.5) / 2)  # Center of output array at dftshift
+        row_shift = dvclib.round(row_shift * usfac) / usfac
+        col_shift = dvclib.round(col_shift * usfac) / usfac
+        dftshift = dvclib.fix(dvclib.ceil(usfac * 1.5) / 2)  # Center of output array at dftshift
         # Matrix multiply DFT around the current shift estimate
-        c_c = dvclib2.conj(dftups(arr * dvclib2.conj(ref_arr), int(math.ceil(usfac * 1.5)), int(math.ceil(usfac * 1.5)), usfac,
+        c_c = dvclib.conj(dftups(arr * dvclib.conj(ref_arr), int(math.ceil(usfac * 1.5)), int(math.ceil(usfac * 1.5)), usfac,
                              int(dftshift - row_shift * usfac), int(dftshift - col_shift * usfac))) / \
               (int(math.trunc(shape[0] / 2)) * int(math.trunc(shape[1] / 2)) * usfac ^ 2)
         # Locate maximum and map back to original pixel grid
-        max_coord = dvclib2.unravel_index(dvclib2.argmax(c_c), dvclib2.dims(c_c))
+        max_coord = dvclib.unravel_index(dvclib.argmax(c_c), dvclib.dims(c_c))
         [rloc, cloc] = max_coord
 
         rloc = rloc - dftshift
         cloc = cloc - dftshift
         row_shift = row_shift + rloc / usfac
         col_shift = col_shift + cloc / usfac
 
@@ -374,17 +367,17 @@
         Fourier transform of image to register
 
     Returns
     -------
     shift_2, shift_1, shift_0 : float, float
         pixel shifts between images
     """
-    r_shift_2, c_shift_2 = dftregistration(dvclib2.fft(dvclib.sum(ref_arr, 2)), dvclib2.fft(dvclib.sum(arr, 2)), 100)
-    r_shift_1, c_shift_1 = dftregistration(dvclib2.fft(dvclib.sum(ref_arr, 1)), dvclib2.fft(dvclib.sum(arr, 1)), 100)
-    r_shift_0, c_shift_0 = dftregistration(dvclib2.fft(dvclib.sum(ref_arr, 0)), dvclib2.fft(dvclib.sum(arr, 0)), 100)
+    r_shift_2, c_shift_2 = dftregistration(dvclib.fft(dvclib.sum(ref_arr, 2)), dvclib.fft(dvclib.sum(arr, 2)), 100)
+    r_shift_1, c_shift_1 = dftregistration(dvclib.fft(dvclib.sum(ref_arr, 1)), dvclib.fft(dvclib.sum(arr, 1)), 100)
+    r_shift_0, c_shift_0 = dftregistration(dvclib.fft(dvclib.sum(ref_arr, 0)), dvclib.fft(dvclib.sum(arr, 0)), 100)
 
     shift_2 = sum([r_shift_2, r_shift_1]) * 0.5
     shift_1 = sum([c_shift_2, r_shift_0]) * 0.5
     shift_0 = sum([c_shift_1, c_shift_0]) * 0.5
     return shift_2, shift_1, shift_0
 
 
@@ -460,57 +453,49 @@
     c_c = dvclib.conj(arr1) * arr2
     c_c_tot = dvclib.sum(c_c)
     ph = dvclib.angle(c_c_tot)
     arr = arr1 * dvclib.exp(1j * ph)
     return arr
 
 
-def breed(breed_mode, parent_dir, image):
+def breed(breed_mode, alpha_dir, image):
     """
     Aligns the image to breed from with the alpha image, and applies breed formula, to obtain a 'child' image.
 
     Parameters
     ----------
     alpha : ndarray
         the best image in the generation
     breed_mode : str
         literal defining the breeding process
     dirs : tuple
         a tuple containing two elements: directory where the image to breed from is stored, a 'parent', and a directory where the bred image, a 'child', will be stored.
 
     """
-    parent_dir = parent_dir.replace(os.sep, '/')
-
     # load alpha from alpha dir
-    alpha = dvclib.load(os.path.dirname(os.path.dirname(parent_dir)) + '/alpha/image.npy')
-    if parent_dir.endswith('0'):  # it is the best, can be the same as alpha
-        if dvclib.sum(image) == dvclib.sum(alpha):
-            # it is alpha, no breeding
-            return zero_phase(image)
-
+    alpha = dvclib.load(alpha_dir + '/image.npy')
+    if dvclib.array_equal(image, alpha):
+        # it is alpha, no breeding
+        return zero_phase(image)
     alpha = zero_phase(alpha)
 
     # load image file
     beta = image
     beta = zero_phase(beta)
     alpha = check_get_conj_reflect(beta, alpha)
     alpha = align_arrays(beta, alpha)
     alpha = zero_phase(alpha)
     ph_alpha = dvclib.angle(alpha)
     beta = zero_phase_cc(beta, alpha)
     ph_beta = dvclib.angle(beta)
     if breed_mode == 'sqrt_ab':
         beta = dvclib.sqrt(dvclib.absolute(alpha) * dvclib.absolute(beta)) * dvclib.exp(0.5j * (ph_beta + ph_alpha))
 
-    elif breed_mode == 'dsqrt':
-        amp = dvclib.sqrt(dvclib.absolute(beta))
-        beta = amp * dvclib.exp(1j * ph_beta)
-
     elif breed_mode == 'pixel_switch':
-        cond = dvclib.random(dvclib.shape(beta))
+        cond = dvclib.random(beta.shape)
         beta = dvclib.where((cond > 0.5), beta, alpha)
 
     elif breed_mode == 'b_pa':
         beta = dvclib.absolute(beta) * dvclib.exp(1j * ph_alpha)
 
     elif breed_mode == '2ab_a_b':
         beta = 2 * (beta * alpha) / (beta + alpha)
@@ -533,69 +518,10 @@
     elif breed_mode == 'max_ab_pa':
         beta = dvclib.maximum(dvclib.absolute(alpha), dvclib.absolute(beta)) * dvclib.exp(1j * ph_alpha)
 
     elif breed_mode == 'avg_ab':
         beta = 0.5 * (alpha + beta)
 
     elif breed_mode == 'avg_ab_pa':
-        beta = 0.5 * (dvclib.absolute(alpha) + dvclib.absolute(beta)) * dvclib.exp(1j * (ph_alpha))
+        beta = 0.5 * (dvclib.absolute(alpha) + dvclib.absolute(beta)) * dvclib.exp(1j * ph_alpha)
 
     return beta
-
-
-# def save_results(image, support, coh, errs, save_dir):
-#     """
-#     Saves results of reconstruction. Saves the following files: image.np, support.npy, errors.npy, optionally coherence.npy, plot_errors.py, graph.npy, flow.npy, iter_array.npy
-#
-#
-#     Parameters
-#     ----------
-#     image : ndarray
-#         reconstructed image array
-#
-#     support : ndarray
-#         support array related to the image
-#
-#     coh : ndarray
-#         coherence array when pcdi feature is active, None otherwise
-#
-#     errs : ndarray
-#         errors "chi" by iterations
-#
-#     flow : ndarray
-#         for development, contains functions that can be activated in fast module during iteration
-#
-#     iter_array : ndarray
-#         for development, matrix indicating which function in fast module was active by iteration
-#
-#     save_dir : str
-#         directory to write the files
-#
-#     metrics : dict
-#         dictionary with metric type keys, and metric values
-#
-#     Returns
-#     -------
-#     nothing
-#     """
-#     print('in save results')
-#     save_dir = save_dir.replace(os.sep, '/')
-#     if not os.path.exists(save_dir):
-#         os.makedirs(save_dir)
-#     image_file = save_dir + '/image'
-#     dvclib.save(image_file, image)
-#     support_file = save_dir + '/support'
-#     dvclib.save(support_file, support)
-#
-#     errs_file = save_dir + '/errors'
-#     dvclib.save(errs_file, errs)
-#     if not coh is None:
-#         coh_file = save_dir + '/coherence'
-#         dvclib.save(coh_file, coh)
-#
-#     print ('will save metrics.txt')
-#     with open(save_dir + "/metrics.txt", "w+") as f:
-#         metric = all_metrics(image, errs)
-#         f.write(metric)
-#         print('saved metris.txt')
-#
-
```

### Comparing `cohere_core-3.2/cohere_core/utilities/utils.py` & `cohere_core-4.0b0/cohere_core/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `cohere_core-3.2/cohere_core.egg-info/SOURCES.txt` & `cohere_core-4.0b0/cohere_core.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -5,25 +5,29 @@
 cohere_core.egg-info/PKG-INFO
 cohere_core.egg-info/SOURCES.txt
 cohere_core.egg-info/dependency_links.txt
 cohere_core.egg-info/requires.txt
 cohere_core.egg-info/top_level.txt
 cohere_core/controller/AI_guess.py
 cohere_core/controller/__init__.py
+cohere_core/controller/features.py
 cohere_core/controller/op_flow.py
 cohere_core/controller/phasing.py
 cohere_core/controller/reconstruction_GA.py
+cohere_core/controller/reconstruction_coupled.py
 cohere_core/controller/reconstruction_multi.py
 cohere_core/controller/reconstruction_single.py
 cohere_core/data/__init__.py
 cohere_core/data/alien_tools.py
+cohere_core/data/auto_prep.py
 cohere_core/data/standard_preprocess.py
 cohere_core/lib/__init__.py
 cohere_core/lib/aflib.py
 cohere_core/lib/cohlib.py
 cohere_core/lib/cplib.py
 cohere_core/lib/nplib.py
+cohere_core/lib/torchlib.py
 cohere_core/utilities/__init__.py
 cohere_core/utilities/config_errors_dict.py
 cohere_core/utilities/config_verifier.py
 cohere_core/utilities/dvc_utils.py
 cohere_core/utilities/utils.py
```

### Comparing `cohere_core-3.2/setup.py` & `cohere_core-4.0b0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 setuptools.setup(
       name='cohere_core',
       author = 'Barbara Frosik, Ross Harder',
       author_email = 'bfrosik@anl.gov',
       url='https://github.com/advancedPhotonSource/cohere',
-      version='3.2',
+      version='4.0-beta',
       packages=setuptools.find_packages(),
       install_requires=['numpy',
-                        'tensorflow',
                         'scikit-learn',
                         'tifffile',
                         ],
       classifiers=[
             'Intended Audience :: Science/Research',
             'Programming Language :: Python :: 3.6',
             'Programming Language :: Python :: 3.7',
             'Programming Language :: Python :: 3.8',
             'Programming Language :: Python :: 3.9',
             'Programming Language :: Python :: 3.10',
+            'Programming Language :: Python :: 3.11',
       ],
 
 )
```

