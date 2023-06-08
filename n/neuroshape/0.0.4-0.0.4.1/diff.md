# Comparing `tmp/neuroshape-0.0.4.tar.gz` & `tmp/neuroshape-0.0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuroshape-0.0.4.tar", last modified: Wed Jun  7 05:26:30 2023, max compression
+gzip compressed data, was "neuroshape-0.0.4.1.tar", last modified: Thu Jun  8 07:37:40 2023, max compression
```

## Comparing `neuroshape-0.0.4.tar` & `neuroshape-0.0.4.1.tar`

### file list

```diff
@@ -1,48 +1,47 @@
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-07 05:26:30.846755 neuroshape-0.0.4/
--rw-r--r--   0 nik        (502) admin       (80)     1501 2023-06-07 02:08:37.000000 neuroshape-0.0.4/LICENSE
--rw-r--r--   0 nik        (502) admin       (80)       70 2023-06-04 23:43:38.000000 neuroshape-0.0.4/MANIFEST.in
--rw-r--r--   0 nik        (502) admin       (80)      466 2023-06-07 05:26:30.846418 neuroshape-0.0.4/PKG-INFO
--rw-r--r--   0 nik        (502) admin       (80)     5334 2023-06-07 03:43:39.000000 neuroshape-0.0.4/README.rst
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-07 05:26:30.836193 neuroshape-0.0.4/neuroshape/
--rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/__init__.py
--rw-r--r--   0 nik        (502) admin       (80)    20918 2023-06-07 04:43:27.000000 neuroshape-0.0.4/neuroshape/connectopic_laplacian.py
--rw-r--r--   0 nik        (502) admin       (80)     5054 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/eigenmaps.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-07 05:26:30.839752 neuroshape-0.0.4/neuroshape/nulls/
--rw-r--r--   0 nik        (502) admin       (80)      347 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/nulls/__init__.py
--rw-r--r--   0 nik        (502) admin       (80)     5351 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/nulls/burt.py
--rw-r--r--   0 nik        (502) admin       (80)    14902 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/nulls/eigenshuff.py
--rw-r--r--   0 nik        (502) admin       (80)    25239 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/nulls/nulls.py
--rw-r--r--   0 nik        (502) admin       (80)    27669 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/nulls/spins.py
--rw-r--r--   0 nik        (502) admin       (80)    12845 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/nulls/waveshuff.py
--rw-r--r--   0 nik        (502) admin       (80)     4078 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/permutation.py
--rw-r--r--   0 nik        (502) admin       (80)     5145 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/poly_eigenmaps.py
--rw-r--r--   0 nik        (502) admin       (80)     5400 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/stats.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-07 05:26:30.845023 neuroshape-0.0.4/neuroshape/utils/
--rw-r--r--   0 nik        (502) admin       (80)       25 2023-06-07 00:31:38.000000 neuroshape-0.0.4/neuroshape/utils/__init__.py
--rw-r--r--   0 nik        (502) admin       (80)     1345 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/utils/check_fs_subjid.py
--rw-r--r--   0 nik        (502) admin       (80)      616 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/utils/check_map.py
--rw-r--r--   0 nik        (502) admin       (80)     6553 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/utils/checks.py
--rw-r--r--   0 nik        (502) admin       (80)      917 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/utils/compare_parallel.py
--rw-r--r--   0 nik        (502) admin       (80)     3501 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/utils/compute_geodesic_distance.py
--rw-r--r--   0 nik        (502) admin       (80)     6248 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/utils/concavehull.py
--rw-r--r--   0 nik        (502) admin       (80)     3428 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/utils/eigen.py
--rw-r--r--   0 nik        (502) admin       (80)    25397 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/utils/fs_shapeDNA.py
--rw-r--r--   0 nik        (502) admin       (80)     9310 2023-06-07 04:41:54.000000 neuroshape-0.0.4/neuroshape/utils/geometry.py
--rw-r--r--   0 nik        (502) admin       (80)      348 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/utils/load_mesh_vertices.py
--rw-r--r--   0 nik        (502) admin       (80)     2639 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/utils/meshtransforms.py
--rw-r--r--   0 nik        (502) admin       (80)      201 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/utils/swap_single_row.py
--rw-r--r--   0 nik        (502) admin       (80)      540 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/utils/tmpname.py
--rw-r--r--   0 nik        (502) admin       (80)      193 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/utils/zscore_avg_method.py
--rw-r--r--   0 nik        (502) admin       (80)    15295 2023-06-07 02:28:43.000000 neuroshape-0.0.4/neuroshape/volume_eigenmodes.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-07 05:26:30.837508 neuroshape-0.0.4/neuroshape.egg-info/
--rw-r--r--   0 nik        (502) admin       (80)      466 2023-06-07 05:26:30.000000 neuroshape-0.0.4/neuroshape.egg-info/PKG-INFO
--rw-r--r--   0 nik        (502) admin       (80)     1102 2023-06-07 05:26:30.000000 neuroshape-0.0.4/neuroshape.egg-info/SOURCES.txt
--rw-r--r--   0 nik        (502) admin       (80)        1 2023-06-07 05:26:30.000000 neuroshape-0.0.4/neuroshape.egg-info/dependency_links.txt
--rw-r--r--   0 nik        (502) admin       (80)       11 2023-06-07 05:26:30.000000 neuroshape-0.0.4/neuroshape.egg-info/top_level.txt
--rw-r--r--   0 nik        (502) admin       (80)      106 2023-06-04 23:43:38.000000 neuroshape-0.0.4/requirements.txt
--rw-r--r--   0 nik        (502) admin       (80)       38 2023-06-07 05:26:30.846849 neuroshape-0.0.4/setup.cfg
--rw-r--r--   0 nik        (502) admin       (80)     1021 2023-06-07 05:26:25.000000 neuroshape-0.0.4/setup.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-07 05:26:30.846010 neuroshape-0.0.4/src/
--rw-r--r--   0 nik        (502) admin       (80)     4664 2023-06-06 23:21:17.000000 neuroshape-0.0.4/src/eta_squared.c
--rw-r--r--   0 nik        (502) admin       (80)     2545 2023-06-06 05:49:54.000000 neuroshape-0.0.4/src/euler_threshold.c
--rw-r--r--   0 nik        (502) admin       (80)     5946 2023-06-06 05:46:53.000000 neuroshape-0.0.4/src/glmfit.c
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-08 07:37:40.326776 neuroshape-0.0.4.1/
+-rw-r--r--   0 nik        (502) admin       (80)     1501 2023-06-07 02:08:37.000000 neuroshape-0.0.4.1/LICENSE
+-rw-r--r--   0 nik        (502) admin       (80)      468 2023-06-08 07:37:40.326508 neuroshape-0.0.4.1/PKG-INFO
+-rw-r--r--   0 nik        (502) admin       (80)     4445 2023-06-08 03:48:59.000000 neuroshape-0.0.4.1/README.rst
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-08 07:37:40.311140 neuroshape-0.0.4.1/neuroshape/
+-rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.1/neuroshape/__init__.py
+-rw-r--r--   0 nik        (502) admin       (80)    21494 2023-06-07 06:22:41.000000 neuroshape-0.0.4.1/neuroshape/connectopic_laplacian.py
+-rw-r--r--   0 nik        (502) admin       (80)     5054 2023-06-04 23:43:38.000000 neuroshape-0.0.4.1/neuroshape/eigenmaps.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-08 07:37:40.316638 neuroshape-0.0.4.1/neuroshape/nulls/
+-rw-r--r--   0 nik        (502) admin       (80)       44 2023-06-08 03:48:59.000000 neuroshape-0.0.4.1/neuroshape/nulls/__init__.py
+-rw-r--r--   0 nik        (502) admin       (80)     5351 2023-06-04 23:43:38.000000 neuroshape-0.0.4.1/neuroshape/nulls/burt.py
+-rw-r--r--   0 nik        (502) admin       (80)    14902 2023-06-04 23:43:38.000000 neuroshape-0.0.4.1/neuroshape/nulls/eigenshuff.py
+-rw-r--r--   0 nik        (502) admin       (80)    11914 2023-06-08 03:48:59.000000 neuroshape-0.0.4.1/neuroshape/nulls/eigensphere.py
+-rw-r--r--   0 nik        (502) admin       (80)    25239 2023-06-04 23:43:38.000000 neuroshape-0.0.4.1/neuroshape/nulls/nulls.py
+-rw-r--r--   0 nik        (502) admin       (80)    27669 2023-06-04 23:43:38.000000 neuroshape-0.0.4.1/neuroshape/nulls/spins.py
+-rw-r--r--   0 nik        (502) admin       (80)    12845 2023-06-04 23:43:38.000000 neuroshape-0.0.4.1/neuroshape/nulls/waveshuff.py
+-rw-r--r--   0 nik        (502) admin       (80)     4078 2023-06-04 23:43:38.000000 neuroshape-0.0.4.1/neuroshape/permutation.py
+-rw-r--r--   0 nik        (502) admin       (80)     5145 2023-06-04 23:43:38.000000 neuroshape-0.0.4.1/neuroshape/poly_eigenmaps.py
+-rw-r--r--   0 nik        (502) admin       (80)     5400 2023-06-04 23:43:38.000000 neuroshape-0.0.4.1/neuroshape/stats.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-08 07:37:40.325254 neuroshape-0.0.4.1/neuroshape/utils/
+-rw-r--r--   0 nik        (502) admin       (80)       25 2023-06-07 00:31:38.000000 neuroshape-0.0.4.1/neuroshape/utils/__init__.py
+-rw-r--r--   0 nik        (502) admin       (80)     1345 2023-06-04 23:43:38.000000 neuroshape-0.0.4.1/neuroshape/utils/check_fs_subjid.py
+-rw-r--r--   0 nik        (502) admin       (80)      616 2023-06-04 23:43:38.000000 neuroshape-0.0.4.1/neuroshape/utils/check_map.py
+-rw-r--r--   0 nik        (502) admin       (80)     6553 2023-06-04 23:43:38.000000 neuroshape-0.0.4.1/neuroshape/utils/checks.py
+-rw-r--r--   0 nik        (502) admin       (80)      917 2023-06-04 23:43:38.000000 neuroshape-0.0.4.1/neuroshape/utils/compare_parallel.py
+-rw-r--r--   0 nik        (502) admin       (80)     3501 2023-06-04 23:43:38.000000 neuroshape-0.0.4.1/neuroshape/utils/compute_geodesic_distance.py
+-rw-r--r--   0 nik        (502) admin       (80)     6248 2023-06-04 23:43:38.000000 neuroshape-0.0.4.1/neuroshape/utils/concavehull.py
+-rw-r--r--   0 nik        (502) admin       (80)    10192 2023-06-08 03:48:59.000000 neuroshape-0.0.4.1/neuroshape/utils/eigen.py
+-rw-r--r--   0 nik        (502) admin       (80)    25397 2023-06-04 23:43:38.000000 neuroshape-0.0.4.1/neuroshape/utils/fs_shapeDNA.py
+-rw-r--r--   0 nik        (502) admin       (80)     9310 2023-06-07 04:41:54.000000 neuroshape-0.0.4.1/neuroshape/utils/geometry.py
+-rw-r--r--   0 nik        (502) admin       (80)      348 2023-06-04 23:43:38.000000 neuroshape-0.0.4.1/neuroshape/utils/load_mesh_vertices.py
+-rw-r--r--   0 nik        (502) admin       (80)     2639 2023-06-04 23:43:38.000000 neuroshape-0.0.4.1/neuroshape/utils/meshtransforms.py
+-rw-r--r--   0 nik        (502) admin       (80)      201 2023-06-04 23:43:38.000000 neuroshape-0.0.4.1/neuroshape/utils/swap_single_row.py
+-rw-r--r--   0 nik        (502) admin       (80)      540 2023-06-04 23:43:38.000000 neuroshape-0.0.4.1/neuroshape/utils/tmpname.py
+-rw-r--r--   0 nik        (502) admin       (80)      193 2023-06-04 23:43:38.000000 neuroshape-0.0.4.1/neuroshape/utils/zscore_avg_method.py
+-rw-r--r--   0 nik        (502) admin       (80)    15295 2023-06-07 02:28:43.000000 neuroshape-0.0.4.1/neuroshape/volume_eigenmodes.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-08 07:37:40.312037 neuroshape-0.0.4.1/neuroshape.egg-info/
+-rw-r--r--   0 nik        (502) admin       (80)      468 2023-06-08 07:37:40.000000 neuroshape-0.0.4.1/neuroshape.egg-info/PKG-INFO
+-rw-r--r--   0 nik        (502) admin       (80)     1105 2023-06-08 07:37:40.000000 neuroshape-0.0.4.1/neuroshape.egg-info/SOURCES.txt
+-rw-r--r--   0 nik        (502) admin       (80)        1 2023-06-08 07:37:40.000000 neuroshape-0.0.4.1/neuroshape.egg-info/dependency_links.txt
+-rw-r--r--   0 nik        (502) admin       (80)       11 2023-06-08 07:37:40.000000 neuroshape-0.0.4.1/neuroshape.egg-info/top_level.txt
+-rw-r--r--   0 nik        (502) admin       (80)       38 2023-06-08 07:37:40.326853 neuroshape-0.0.4.1/setup.cfg
+-rw-r--r--   0 nik        (502) admin       (80)     1063 2023-06-08 07:37:35.000000 neuroshape-0.0.4.1/setup.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-08 07:37:40.326123 neuroshape-0.0.4.1/src/
+-rw-r--r--   0 nik        (502) admin       (80)     5389 2023-06-07 07:20:28.000000 neuroshape-0.0.4.1/src/eta_squared.c
+-rw-r--r--   0 nik        (502) admin       (80)     2545 2023-06-06 05:49:54.000000 neuroshape-0.0.4.1/src/euler_threshold.c
+-rw-r--r--   0 nik        (502) admin       (80)     5946 2023-06-06 05:46:53.000000 neuroshape-0.0.4.1/src/glmfit.c
```

### Comparing `neuroshape-0.0.4/LICENSE` & `neuroshape-0.0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4/README.rst` & `neuroshape-0.0.4.1/README.rst`

 * *Files 21% similar despite different names*

```diff
@@ -19,37 +19,35 @@
 **VERY IMPORTANT:**
 
 In order to use much of the functionality of this code, you must:
 
 1. Install `FreeSurfer <https://surfer.nmr.mgh.harvard.edu/fswiki/DownloadAndInstall>`_ and source it on your OS path.
 2. Install `Connectome Workbench <https://www.humanconnectome.org/software/get-connectome-workbench>`_ and source it on your OS path.
 3. Install `Gmsh <https://gmsh.info/>`_ and source it on your OS path.
-4. Install `MRtrix3 <https://github.com/MRtrix3/mrtrix3>`_ and both source the ``<MRtrix3 installation directory>/bin`` folder on your OS path.
-5. run ``export MRTRIX=<MRtrix3 installation directory>``.
+4. Install `MRtrix3 <https://github.com/MRtrix3/mrtrix3>`_ and source the ``<MRtrix3 installation directory>/bin`` folder on your OS path.
+5. Run ``export MRTRIX=<MRtrix3 installation directory>``.
 6. Source MATLAB on your OS path.
 7. Install `scikit-sparse's libraries <https://github.com/scikit-sparse/scikit-sparse>`_. Follow the installation process over there first.
 
 `See instructions here on how to source binaries to path. <https://superuser.com/questions/284342/what-are-path-and-other-environment-variables-and-how-can-i-set-or-use-them>`_
 
 The ``python`` script ``volume_eigenmodes.py`` was sourced from the `BrainEigenmodes <https://github.com/NSBLab/BrainEigenmodes/tree/main>`_ repository. Please cite their `Nature paper (Pang et al. 2023) <https://www.nature.com/articles/s41586-023-06098-1>`_ if you use that.
 
 The MATLAB scripts in ``neuroshape/functions/wishart`` were sourced from the `HCPpipelines repository <https://github.com/Washington-University/HCPpipelines/tree/master/global/matlab/icaDim>`_ and related `Neuroimage paper (Glasser et al. 2013) <https://pubmed.ncbi.nlm.nih.gov/23668970/>`_. Please be sure to cite them if you use the ``--filter`` functionality in ``connectopic_laplacian.py``.
 
 Installation
 ------------
 
-We have made it easy to download from source and install the dependencies automatically through a ``conda`` environment file (`install and initialize conda first <https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html>`_):
+After installing the above dependencies, install the neuroshape toolbox with:
 
 .. code-block:: bash
   
-  $ git clone https://github.com/breakspear/neuroshape
-  $ cd neuroshape
-  $ conda env create -f environment.yml
+  $ pip install neuroshape
 
-To install scikit-sparse, however, as mentioned above, you will have to `follow their instructions first to install the libraries they depend on <https://github.com/scikit-sparse/scikit-sparse>`_. Come back here when you've done that, then type the above code into a terminal. This will "automatically" (tested and working on MacOS Big Sur v11.6 and MacOS Catalina 10.15.7) download and install the dependencies in an environment called ``neuroshape`` (unless this already exists somehow, in which case you will have to specify your own environment name with ``conda env create -f environment.yml -n myenvironment``).  After downloading the dependencies, several C extensions must be built from source to use:
+You can also compile from source (and install the dependencies automatically):
 
 .. code-block:: bash
 
   $ git clone https://github.com/breakspear/neuroshape
   $ cd neuroshape
   $ conda env create -f environment.yml
   $ python setup.py build
```

### Comparing `neuroshape-0.0.4/neuroshape/connectopic_laplacian.py` & `neuroshape-0.0.4.1/neuroshape/connectopic_laplacian.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 
 new_data = zeros(size(gm_msk,1), size(gm_msk,2), size(gm_msk,3), T);
 [xx, yy, zz] = ind2sub(size(gm_msk), ind_gm);
 
 x = x';
 
 for i = 1:length(ind_gm)
-    new_data(xx(i), yy(i), zz(i), :) = x(i);
+    new_data(xx(i), yy(i), zz(i), :) = x(i,:);
 end
 
 mat2nii(new_data, [folder, '/', basename, '_filtered.nii'], size(new_data), 32, '{mask_filename}');
                    """)
     
     # run matlab at command line
     matpath = [f'{matlabpath}']
@@ -210,23 +210,24 @@
 def calc_gradients(img_input, img_roi, img_mask, num_gradients=2):
     smat = compute_similarity(img_input, img_roi, img_mask)
     
     L = calc_LaplacianMatrix(smat, num_gradients)
     
     evals, egrads = eigh(L)
     
+    # exclude the first eigenvalue, return only the non-zero `num_gradients` last gradients
+    egrads = egrads[:, 1:num_gradients+1]
+    evals = evals[1:num_gradients+1]
+    
     # Z-transform eigenvectors
-    egrads = (egrads - np.mean(egrads))/np.std(egrads)
+    egrads = normalize_data(egrads)
     
     # make positive
     egrads = egrads - np.min(egrads)
     
-    # exclude the first eigenvalue, return only the non-zero `num_gradients` last gradients
-    egrads = egrads[:, 1:num_gradients+1]
-    evals = evals[1:num_gradients+1]
     
     return evals, egrads
 
 def cortical_projection(img_input, img_roi, img_mask, egrads):
     data_msk = masking.apply_mask(img_input, img_mask)
     data_msk = normalize_data(data_msk)
     input_img = masking.unmask(data_msk, img_mask)
@@ -303,16 +304,30 @@
         Flag whether to plot gradient figures. The default is True.
 
     """
     if fwhm:
         print('Smoothing with Gaussian kernel of FWHM = {}mm'.format(fwhm))
         data_input_filename = smooth(data_input_filename, fwhm)
     if filtering is True:
+        print("Normalizing input data before filtering")
+        img_input = image.load_img(data_input_filename)
+        img_mask = image.load_img(mask_filename)
+        
+        # mask and normalize input data
+        data_msk = masking.apply_mask(img_input, img_mask)
+        data_msk = normalize_data(data_msk)
+        img_input = masking.unmask(data_msk, img_mask)
+        
+        output_filename = data_input_filename.replace('.nii', '_normalized.nii')
+        
+        print('Saving normalized data to {}'.format(output_filename))
+        nib.save(img_input, output_filename)
+        
         print('Performing Wishart filtering using icaDim.m, see: <https://github.com/Washington-University/HCPpipelines/tree/master/global/matlab/icaDim>')
-        data_input_filename = wishart(data_input_filename, mask_filename)
+        data_input_filename = wishart(output_filename, mask_filename)
     
     print('Loading images')
     img_input = image.load_img(data_input_filename)
     img_roi = image.load_img(data_roi_filename)
     img_mask = image.load_img(mask_filename)
     
     evals, egrads = calc_gradients(img_input, img_roi, img_mask, num_gradients)
```

### Comparing `neuroshape-0.0.4/neuroshape/eigenmaps.py` & `neuroshape-0.0.4.1/neuroshape/eigenmaps.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4/neuroshape/nulls/burt.py` & `neuroshape-0.0.4.1/neuroshape/nulls/burt.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4/neuroshape/nulls/eigenshuff.py` & `neuroshape-0.0.4.1/neuroshape/nulls/eigenshuff.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4/neuroshape/nulls/nulls.py` & `neuroshape-0.0.4.1/neuroshape/nulls/nulls.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4/neuroshape/nulls/spins.py` & `neuroshape-0.0.4.1/neuroshape/nulls/spins.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4/neuroshape/nulls/waveshuff.py` & `neuroshape-0.0.4.1/neuroshape/nulls/waveshuff.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4/neuroshape/permutation.py` & `neuroshape-0.0.4.1/neuroshape/permutation.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4/neuroshape/poly_eigenmaps.py` & `neuroshape-0.0.4.1/neuroshape/poly_eigenmaps.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4/neuroshape/stats.py` & `neuroshape-0.0.4.1/neuroshape/stats.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4/neuroshape/utils/check_fs_subjid.py` & `neuroshape-0.0.4.1/neuroshape/utils/check_fs_subjid.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4/neuroshape/utils/check_map.py` & `neuroshape-0.0.4.1/neuroshape/utils/check_map.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4/neuroshape/utils/checks.py` & `neuroshape-0.0.4.1/neuroshape/utils/checks.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4/neuroshape/utils/compare_parallel.py` & `neuroshape-0.0.4.1/neuroshape/utils/compare_parallel.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4/neuroshape/utils/compute_geodesic_distance.py` & `neuroshape-0.0.4.1/neuroshape/utils/compute_geodesic_distance.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4/neuroshape/utils/concavehull.py` & `neuroshape-0.0.4.1/neuroshape/utils/concavehull.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4/neuroshape/utils/fs_shapeDNA.py` & `neuroshape-0.0.4.1/neuroshape/utils/fs_shapeDNA.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4/neuroshape/utils/geometry.py` & `neuroshape-0.0.4.1/neuroshape/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4/neuroshape/utils/meshtransforms.py` & `neuroshape-0.0.4.1/neuroshape/utils/meshtransforms.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4/neuroshape/utils/tmpname.py` & `neuroshape-0.0.4.1/neuroshape/utils/tmpname.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4/neuroshape/volume_eigenmodes.py` & `neuroshape-0.0.4.1/neuroshape/volume_eigenmodes.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4/neuroshape.egg-info/SOURCES.txt` & `neuroshape-0.0.4.1/neuroshape.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 LICENSE
-MANIFEST.in
 README.rst
-requirements.txt
 setup.py
 neuroshape/__init__.py
 neuroshape/connectopic_laplacian.py
 neuroshape/eigenmaps.py
 neuroshape/permutation.py
 neuroshape/poly_eigenmaps.py
 neuroshape/stats.py
@@ -13,14 +11,15 @@
 neuroshape.egg-info/PKG-INFO
 neuroshape.egg-info/SOURCES.txt
 neuroshape.egg-info/dependency_links.txt
 neuroshape.egg-info/top_level.txt
 neuroshape/nulls/__init__.py
 neuroshape/nulls/burt.py
 neuroshape/nulls/eigenshuff.py
+neuroshape/nulls/eigensphere.py
 neuroshape/nulls/nulls.py
 neuroshape/nulls/spins.py
 neuroshape/nulls/waveshuff.py
 neuroshape/utils/__init__.py
 neuroshape/utils/check_fs_subjid.py
 neuroshape/utils/check_map.py
 neuroshape/utils/checks.py
```

### Comparing `neuroshape-0.0.4/setup.py` & `neuroshape-0.0.4.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,14 @@
                    include_dirs=[numpy.get_include()])
 
 euler = Extension('neuroshape.euler', sources=['src/euler_threshold.c'],
                   include_dirs=[numpy.get_include()])
 
 # run the setup
 setup(name='neuroshape',
-      version='0.0.4',
+      version='0.0.4.1',
       description="For computing connectopic and geometric Laplacian eigenmodes and performing null hypothesis testing. As implementation is ongoing, this description is subject to rapid change.",
       author='Nikitas C. Koussis, Systems Neuroscience Group Newcastle',
       author_email='nikitas.koussis@gmail.com',
       url='https://github.com/nikitas-k/neuroshape-dev',
-      packages=['neuroshape'],
+      packages=['neuroshape', 'neuroshape.nulls', 'neuroshape.utils'],
       ext_modules=[eta, glmfit, euler])
```

### Comparing `neuroshape-0.0.4/src/eta_squared.c` & `neuroshape-0.0.4.1/src/eta_squared.c`

 * *Files 16% similar despite different names*

```diff
@@ -24,119 +24,135 @@
  *
  * For this program to work, numpy.vectorize must be called in
  * in python to generate a numpy-friendly function. See 
  * neuroshape/examples/compute_eta_squared.py for an example
  * 
  */
 
-/* declare main function */
-static PyObject* eta_squared(PyObject* self, PyObject* args);
-
-/*
- * This tells Python what methods this module has
- *
- */
-static PyMethodDef EtaMethods[] = {
-    {"eta_squared",
-        eta_squared,
-        METH_VARARGS, "Compute eta-squared coefficient row-wise of a 2-dimensional array."},
-    {NULL, NULL, 0, NULL}
-};
-
 /*
  * This actually defines the eta squared function for
  * input args from Python.
  */
 
 
 static PyObject* eta_squared(PyObject* self, PyObject* args)
 {
     PyArrayObject* arr;
     if (!PyArg_ParseTuple(args, "O!", &PyArray_Type, &arr))
         return NULL;
     
-    int num_rows = arr->dimensions[0];
-    int num_cols = arr->dimensions[1];
+    int N = arr->dimensions[0];
+    int p = arr->dimensions[1];
+    
     /* check number of dims and whether data is in correct format */
-    if ( num_rows < num_cols ) {
+    if ( N < p ) {
         printf('ERROR: Number of observations must exceed number of features (is your data transposed?)');
         return NULL;    
     }
     npy_intp nd = PyArray_NDIM(arr);
     if ( nd != 2 ) {
         printf('ERROR: Input must be a 2-dimensional matrix');
         return NULL;    
     }
     
-    npy_intp dims[2] = {num_rows, num_rows};
+    npy_intp dims[2] = {N, N};
 
     PyArrayObject* oarr = (PyArrayObject*)PyArray_SimpleNew(nd, dims, NPY_DOUBLE);
     if (oarr == NULL)
         return NULL;
 
-    double* data_ptr = PyArray_DATA(arr);
-    double* out_ptr = PyArray_DATA(oarr);
+    double* z = PyArray_DATA(arr);
+    double* eta = PyArray_DATA(oarr);
 
-    double mu_bar = 0.0;
-    double mu_1 = 0.0;
-    int count = 0;
+    double* mu = (double*)malloc(N * p * sizeof(double));
+    double* mu_bar = (double*)malloc(N * sizeof(double));
     
     npy_intp row_stride = PyArray_STRIDE(arr, 0) / sizeof(double);
     npy_intp col_stride = PyArray_STRIDE(arr, 1) / sizeof(double);
+    npy_intp outrow_stride = PyArray_STRIDE(oarr, 0) / sizeof(double);
+    npy_intp outcol_stride = PyArray_STRIDE(oarr, 1) / sizeof(double);
     
-    npy_intp i,j,k;
+    for (int i = 0; i < N; i++) {
+        // Calculate mu
+        for (int k = 0; k < p; k++) {
+            double sum = 0.0;
+            for (int j = 0; j < N; j++) {
+                if (j != i)
+                    sum += z[j * row_stride + k * col_stride];
+            }
+            mu[k] = (z[i * row_stride + k * col_stride] + sum) / N;
+        }
+
 
-    // Calculate mu_bar
-    for (i = 0; i < num_rows; i++) {
-        for (k = 0; k < num_rows; k++) {
-            for (j = 0; j < num_cols; j++) {
-                double vali = data_ptr[i * row_stride + j * col_stride];
-                double valk = data_ptr[k * row_stride + j * col_stride];
-                double mu = (vali + valk) / 2.0;
-                mu_1 += mu;
-                count++;
+        // Calculate mu_bar
+        for (int k = 0; k < p; k++) {
+            double sum = 0.0;
+            for (int j = 0; j < N; j++) {
+                sum += z[j * p + k];
             }
+            mu_bar[k] = sum / N;
         }
-    }
-    mu_bar = mu_1 / count;
 
-    // Calculate eta-squared coefficients
-    for (i = 0; i < num_rows; i++) {
-        for (k = 0; k < num_rows; k++) {
+        // Calculate eta_squared
+        for (int j = 0; j < N; j++) {
             double num = 0.0;
             double denom = 0.0;
-            for (j = 0; j < num_cols; j++) {
-                double vali = data_ptr[i * row_stride + j * col_stride];
-                double valk = data_ptr[k * row_stride + j * col_stride];
-                double mu = (vali + valk) / 2.0;
-                double diff_a = vali - mu;
-                double diff_b = valk - mu;
-                double powera = diff_a * diff_a;
-                double powerb = diff_b * diff_b;
-                double diff_bar_a = vali - mu_bar;
-                double diff_bar_b = valk - mu_bar;
-                double powerax = diff_bar_a * diff_bar_a;
-                double powerbx = diff_bar_b * diff_bar_b;
-                num += powera + powerb;
-                denom += powerax + powerbx;
-            }
-            if ( denom == 0.0 ){
-                double eta = 0.0;
-                out_ptr[i*num_rows + k] = eta;
-            } else {
-                double eta = 1.0 - (num / denom);
-                out_ptr[i*num_rows + k] = eta;
+            for (int k = 0; k < p; k++) {
+                double diff = z[i * row_stride + k * col_stride] - mu[k];
+                num += diff * diff;
+                double diff_bar = z[j * row_stride + k * col_stride] - mu_bar[k];
+                denom += diff_bar * diff_bar;
             }
-            
+            eta[j * outrow_stride + i * outcol_stride] = 1.0 - (num / denom);
         }
     }
 
-    Py_DECREF(out_ptr);
+    free(mu);
+    free(mu_bar);
+
     return PyArray_Return(oarr);
 }
+//     // Calculate eta-squared coefficients
+//     for (i = 0; i < num_rows; i++) {
+//         for (k = 0; k < num_rows; k++) {
+//             double num = 0.0;
+//             double denom = 0.0;
+//             for (j = 0; j < num_cols; j++) {
+//                 double vali = data_ptr[i * row_stride + j * col_stride];
+//                 double valk = data_ptr[k * row_stride + j * col_stride];
+//                 double mu = (vali + valk) / 2.0;
+//                 double diff_a = vali - mu;
+//                 double diff_b = valk - mu;
+//                 double powera = diff_a * diff_a;
+//                 double powerb = diff_b * diff_b;
+//                 double diff_bar_a = vali - mu_bar;
+//                 double diff_bar_b = valk - mu_bar;
+//                 double powerax = diff_bar_a * diff_bar_a;
+//                 double powerbx = diff_bar_b * diff_bar_b;
+//                 num += powera + powerb;
+//                 denom += powerax + powerbx;
+//             }
+//             if ( denom == 0.0 ){
+//                 double eta = 0.0;
+//                 out_ptr[i*num_rows + k] = eta;
+//             } else {
+//                 double eta = 1.0 - (num / denom);
+//                 out_ptr[i*num_rows + k] = eta;
+//             }
+//             
+//         }
+//     }
+
+
+static PyMethodDef EtaMethods[] = {
+    {"eta_squared",
+        eta_squared,
+        METH_VARARGS, "Compute eta-squared coefficient row-wise of a 2-dimensional array."},
+    {NULL, NULL, 0, NULL}
+};
 
 static struct PyModuleDef cModPyDem = {
     PyModuleDef_HEAD_INIT,
     "neuroshape.eta",
     "Eta-squared 2-dimensional array calculation implementation in C",
     -1,
     EtaMethods
```

### Comparing `neuroshape-0.0.4/src/euler_threshold.c` & `neuroshape-0.0.4.1/src/euler_threshold.c`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4/src/glmfit.c` & `neuroshape-0.0.4.1/src/glmfit.c`

 * *Files identical despite different names*

