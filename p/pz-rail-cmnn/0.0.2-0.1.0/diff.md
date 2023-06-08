# Comparing `tmp/pz-rail-cmnn-0.0.2.tar.gz` & `tmp/pz-rail-cmnn-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz-rail-cmnn-0.0.2.tar", last modified: Thu Jun  1 00:56:13 2023, max compression
+gzip compressed data, was "pz-rail-cmnn-0.1.0.tar", last modified: Thu Jun  8 00:20:09 2023, max compression
```

## Comparing `pz-rail-cmnn-0.0.2.tar` & `pz-rail-cmnn-0.1.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:56:13.943436 pz-rail-cmnn-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:56:13.939436 pz-rail-cmnn-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:56:13.939436 pz-rail-cmnn-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-01 00:55:59.000000 pz-rail-cmnn-0.0.2/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-01 00:55:59.000000 pz-rail-cmnn-0.0.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-01 00:55:59.000000 pz-rail-cmnn-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-01 00:55:59.000000 pz-rail-cmnn-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-06-01 00:56:13.943436 pz-rail-cmnn-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-06-01 00:55:59.000000 pz-rail-cmnn-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:56:13.939436 pz-rail-cmnn-0.0.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    15280 2023-06-01 00:55:59.000000 pz-rail-cmnn-0.0.2/examples/CMNN_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-06-01 00:55:59.000000 pz-rail-cmnn-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 00:56:13.943436 pz-rail-cmnn-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 00:55:59.000000 pz-rail-cmnn-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:56:13.939436 pz-rail-cmnn-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:56:13.939436 pz-rail-cmnn-0.0.2/src/pz_rail_cmnn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-06-01 00:56:13.000000 pz-rail-cmnn-0.0.2/src/pz_rail_cmnn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-01 00:56:13.000000 pz-rail-cmnn-0.0.2/src/pz_rail_cmnn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 00:56:13.000000 pz-rail-cmnn-0.0.2/src/pz_rail_cmnn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-01 00:56:13.000000 pz-rail-cmnn-0.0.2/src/pz_rail_cmnn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-01 00:56:13.000000 pz-rail-cmnn-0.0.2/src/pz_rail_cmnn.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:56:13.939436 pz-rail-cmnn-0.0.2/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:56:13.943436 pz-rail-cmnn-0.0.2/src/rail/cmnn/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-01 00:55:59.000000 pz-rail-cmnn-0.0.2/src/rail/cmnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-01 00:56:13.000000 pz-rail-cmnn-0.0.2/src/rail/cmnn/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:56:13.939436 pz-rail-cmnn-0.0.2/src/rail/estimation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:56:13.943436 pz-rail-cmnn-0.0.2/src/rail/estimation/algos/
--rw-r--r--   0 runner    (1001) docker     (123)    12632 2023-06-01 00:55:59.000000 pz-rail-cmnn-0.0.2/src/rail/estimation/algos/cmnn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:56:13.943436 pz-rail-cmnn-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-06-01 00:55:59.000000 pz-rail-cmnn-0.0.2/tests/test_algos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-01 00:55:59.000000 pz-rail-cmnn-0.0.2/tests/test_algos.py~
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:20:09.585116 pz-rail-cmnn-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:20:09.585116 pz-rail-cmnn-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:20:09.585116 pz-rail-cmnn-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-08 00:19:59.000000 pz-rail-cmnn-0.1.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-08 00:19:59.000000 pz-rail-cmnn-0.1.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-08 00:19:59.000000 pz-rail-cmnn-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-08 00:19:59.000000 pz-rail-cmnn-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-06-08 00:20:09.585116 pz-rail-cmnn-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-06-08 00:19:59.000000 pz-rail-cmnn-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:20:09.585116 pz-rail-cmnn-0.1.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    16883 2023-06-08 00:19:59.000000 pz-rail-cmnn-0.1.0/examples/CMNN_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-06-08 00:19:59.000000 pz-rail-cmnn-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 00:20:09.585116 pz-rail-cmnn-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 00:19:59.000000 pz-rail-cmnn-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:20:09.585116 pz-rail-cmnn-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:20:09.585116 pz-rail-cmnn-0.1.0/src/pz_rail_cmnn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-06-08 00:20:09.000000 pz-rail-cmnn-0.1.0/src/pz_rail_cmnn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-08 00:20:09.000000 pz-rail-cmnn-0.1.0/src/pz_rail_cmnn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 00:20:09.000000 pz-rail-cmnn-0.1.0/src/pz_rail_cmnn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-08 00:20:09.000000 pz-rail-cmnn-0.1.0/src/pz_rail_cmnn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-08 00:20:09.000000 pz-rail-cmnn-0.1.0/src/pz_rail_cmnn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:20:09.585116 pz-rail-cmnn-0.1.0/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:20:09.585116 pz-rail-cmnn-0.1.0/src/rail/cmnn/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-08 00:19:59.000000 pz-rail-cmnn-0.1.0/src/rail/cmnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-08 00:20:09.000000 pz-rail-cmnn-0.1.0/src/rail/cmnn/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:20:09.585116 pz-rail-cmnn-0.1.0/src/rail/estimation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:20:09.585116 pz-rail-cmnn-0.1.0/src/rail/estimation/algos/
+-rw-r--r--   0 runner    (1001) docker     (123)    14917 2023-06-08 00:19:59.000000 pz-rail-cmnn-0.1.0/src/rail/estimation/algos/cmnn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:20:09.585116 pz-rail-cmnn-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-08 00:19:59.000000 pz-rail-cmnn-0.1.0/tests/test_algos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-08 00:19:59.000000 pz-rail-cmnn-0.1.0/tests/test_algos.py~
```

### Comparing `pz-rail-cmnn-0.0.2/.github/workflows/main.yml` & `pz-rail-cmnn-0.1.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-cmnn-0.0.2/.github/workflows/publish-to-pypi.yml` & `pz-rail-cmnn-0.1.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-cmnn-0.0.2/.gitignore` & `pz-rail-cmnn-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pz-rail-cmnn-0.0.2/LICENSE` & `pz-rail-cmnn-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pz-rail-cmnn-0.0.2/PKG-INFO` & `pz-rail-cmnn-0.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-cmnn
-Version: 0.0.2
+Version: 0.1.0
 Summary: RAIL CMNN Interface
 Author-email: The LSST DESC PZ WG <samuel.j.schmidt@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,22 +43,25 @@
 RAIL interface to Melissa Graham's CMNN algorithm.  A slight modification of the original code found here: <br>
 [dirac-institute/CMNN_Photoz_estimator](https://github.com/dirac-institute/CMNN_Photoz_Estimator)
 
 See https://ui.adsabs.harvard.edu/abs/2018AJ....155....1G/abstract
 for more details on the code
 Any use of `rail_cmnn` in a paper or report should cite [Graham et al. (2018)](https://ui.adsabs.harvard.edu/abs/2018AJ....155....1G/abstract).
 
-The current version of the code consists of a training stage, `Inform_CMNNPDF`, that computes colors for a set of training data (replacing non-detections with the 1-sigma limiting magnitude), and an estimation stage `CMNNPDF` that calculates the Mahalanobis distance to each training galaxy for each test galaxy and returns a single Guassian PDF for each galaxy where the mean can be estimated in one of three ways (see `selection mode` below), and the width is determined by the standard deviation of training galaxy redshifts within the threshold Mahalanobis distance.  Future implementation improvements may change the output format to include multiple Gaussians.
+The current version of the code consists of a training stage, `Inform_CMNNPDF`, that computes colors for a set of training data and an estimation stage `CMNNPDF` that calculates the Mahalanobis distance to each training galaxy for each test galaxy. The mean value of this Guassian PDF can be estimated in one of three ways (see `selection mode` below), and the width is determined by the standard deviation of training galaxy redshifts within the threshold Mahalanobis distance.  Future implementation improvements may change the output format to include multiple Gaussians.
+
+For the color calculation, there is an option for how to treat the "non-detections" in a band: the default choice is to ignore any colors that contain a non-detect magnitude and adjust the number of degrees of freedom in the Mahalanobis distance accordingly (this is how the CMNN algorithm was originally implemented). Or, if the configuration parameter `nondetect_replace` is set to `True` in `Inform_CMNNPDF`, the non-detected magnitudes will be replaced with the 1-sigma limiting magnitude in each band as supplied by the user via the `mag_limits` configuration parameter (or by the default 1-sigma limits if the user does not supply specific numbers). We have not done any exploration of the relative performance of these two choices, but note that there is not a significant performance difference in terms of runtime between the two methods.
 
 `Inform_CMNNPDF` takes in a training data set and returns a model file that simply consists of the computed colors and color errors (magnitude errors added in quadrature) for that dataset, the model to be used in the `CMNNPDF` stage. A modification of the original CMNN algorithm, "nondetections" are now replaced by the 1-sigma limiting magnitudes and the non-detect magnitude errors replaced with a value of 1.0.  The config parameters that can be set by the user for `Inform_CMNNPDF` are:<br>
 - `bands`: list of the band names that should be present in the input data.<br>
 - `err_bands`: list of the magnitude error column names that should be present in the input data.<br>
 - `redshift_col`: a string giving the name for the redshift column present in the input data.<br>
 - `mag_limits`: a dictionary with keys that match those in `bands` and a float with the 1 sigma limiting magnitude for each band.<br>
 - nondetect_val: float or `np.nan`, the value indicating a non-detection, which will be replaced by the values in `mag_limits`.<br>
+- `nondetect_replace`: bool, if set to False (the default) this option ignores colors with non-detected values in the Mahalanobis distance calculation, with a corresponding drop in the degrees of freedom value. If set to True, the method will replace non-detections with the 1-sigma limiting magnitudes specified via `mag_limits` (or default 1-sigma limits if not supplied), and will use all colors in the Mahalanobis distance calculation.
 
 
 The parameters that can be set via the `config_params` in `CMNNPDF` are described in brief below:<br>
 - `bands`, `err_bands`, `redshift_col`, `mag_limits` are all the same as described above for `Inform_CMNNPDF.`<br>
 - `ppf_value`: float, usually 0.68 or 0.95, which sets the value of the PPF used in the Mahalanobis distance calculation.<br>
 - `selection_mode`: int, selects how the central value of the Gaussian PDF is calculated in the algorithm, if set to `0` randomly chooses from set within the Mahalanobis distance, if set to `1` chooses the nearest neighbor point, if set to `2` adds a distance weight to the random choice.<br>
 - `min_n`: int, the minimum number of training galaxies to use.<br>
```

### Comparing `pz-rail-cmnn-0.0.2/README.md` & `pz-rail-cmnn-0.1.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -2,22 +2,25 @@
 RAIL interface to Melissa Graham's CMNN algorithm.  A slight modification of the original code found here: <br>
 [dirac-institute/CMNN_Photoz_estimator](https://github.com/dirac-institute/CMNN_Photoz_Estimator)
 
 See https://ui.adsabs.harvard.edu/abs/2018AJ....155....1G/abstract
 for more details on the code
 Any use of `rail_cmnn` in a paper or report should cite [Graham et al. (2018)](https://ui.adsabs.harvard.edu/abs/2018AJ....155....1G/abstract).
 
-The current version of the code consists of a training stage, `Inform_CMNNPDF`, that computes colors for a set of training data (replacing non-detections with the 1-sigma limiting magnitude), and an estimation stage `CMNNPDF` that calculates the Mahalanobis distance to each training galaxy for each test galaxy and returns a single Guassian PDF for each galaxy where the mean can be estimated in one of three ways (see `selection mode` below), and the width is determined by the standard deviation of training galaxy redshifts within the threshold Mahalanobis distance.  Future implementation improvements may change the output format to include multiple Gaussians.
+The current version of the code consists of a training stage, `Inform_CMNNPDF`, that computes colors for a set of training data and an estimation stage `CMNNPDF` that calculates the Mahalanobis distance to each training galaxy for each test galaxy. The mean value of this Guassian PDF can be estimated in one of three ways (see `selection mode` below), and the width is determined by the standard deviation of training galaxy redshifts within the threshold Mahalanobis distance.  Future implementation improvements may change the output format to include multiple Gaussians.
+
+For the color calculation, there is an option for how to treat the "non-detections" in a band: the default choice is to ignore any colors that contain a non-detect magnitude and adjust the number of degrees of freedom in the Mahalanobis distance accordingly (this is how the CMNN algorithm was originally implemented). Or, if the configuration parameter `nondetect_replace` is set to `True` in `Inform_CMNNPDF`, the non-detected magnitudes will be replaced with the 1-sigma limiting magnitude in each band as supplied by the user via the `mag_limits` configuration parameter (or by the default 1-sigma limits if the user does not supply specific numbers). We have not done any exploration of the relative performance of these two choices, but note that there is not a significant performance difference in terms of runtime between the two methods.
 
 `Inform_CMNNPDF` takes in a training data set and returns a model file that simply consists of the computed colors and color errors (magnitude errors added in quadrature) for that dataset, the model to be used in the `CMNNPDF` stage. A modification of the original CMNN algorithm, "nondetections" are now replaced by the 1-sigma limiting magnitudes and the non-detect magnitude errors replaced with a value of 1.0.  The config parameters that can be set by the user for `Inform_CMNNPDF` are:<br>
 - `bands`: list of the band names that should be present in the input data.<br>
 - `err_bands`: list of the magnitude error column names that should be present in the input data.<br>
 - `redshift_col`: a string giving the name for the redshift column present in the input data.<br>
 - `mag_limits`: a dictionary with keys that match those in `bands` and a float with the 1 sigma limiting magnitude for each band.<br>
 - nondetect_val: float or `np.nan`, the value indicating a non-detection, which will be replaced by the values in `mag_limits`.<br>
+- `nondetect_replace`: bool, if set to False (the default) this option ignores colors with non-detected values in the Mahalanobis distance calculation, with a corresponding drop in the degrees of freedom value. If set to True, the method will replace non-detections with the 1-sigma limiting magnitudes specified via `mag_limits` (or default 1-sigma limits if not supplied), and will use all colors in the Mahalanobis distance calculation.
 
 
 The parameters that can be set via the `config_params` in `CMNNPDF` are described in brief below:<br>
 - `bands`, `err_bands`, `redshift_col`, `mag_limits` are all the same as described above for `Inform_CMNNPDF.`<br>
 - `ppf_value`: float, usually 0.68 or 0.95, which sets the value of the PPF used in the Mahalanobis distance calculation.<br>
 - `selection_mode`: int, selects how the central value of the Gaussian PDF is calculated in the algorithm, if set to `0` randomly chooses from set within the Mahalanobis distance, if set to `1` chooses the nearest neighbor point, if set to `2` adds a distance weight to the random choice.<br>
 - `min_n`: int, the minimum number of training galaxies to use.<br>
```

### Comparing `pz-rail-cmnn-0.0.2/examples/CMNN_demo.ipynb` & `pz-rail-cmnn-0.1.0/examples/CMNN_demo.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994353991596638%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(3, 'last run successfully: June 7, 2023<br>\\n'), (9, 'The "*

 * *            'current version of the code consists of a training stage, `Inform_CMNNPDF`, that '*

 * *            'computes colors for a set of training data and an estimation stage `CMNNPDF` that '*

 * *            'calculates the Mahalanobis distance to each training galaxy for each test galaxy and '*

 * *            'returns a single Guassian PDF for each galaxy.   The mean value of this Gaussian PDF '*

 * *            'can be […]*

```diff
@@ -3,31 +3,34 @@
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# RAIL CMNN Tutorial Notebook\n",
                 "\n",
                 "author: Sam Schmidt<br>\n",
-                "last run successfully: May 31, 2023<br>\n",
+                "last run successfully: June 7, 2023<br>\n",
                 "\n",
                 "This is a notebook demonstrating some of the features of the LSSTDESC `RAIL` version of the CMNN estimator, see **[Graham et al. (2018)](https://ui.adsabs.harvard.edu/abs/2018AJ....155....1G/abstract)** for more details on the algorithm.<br>\n",
                 "\n",
                 "CMNN stands for color-matched nearest-neighbor, and as this name implies, the method works by finding the Mahalanobis distance between each test galaxy and the training galaxies, and selecting one of those \"nearby\" in color space as the redshift estimate.  The algorithm also estimates the \"width\" of the resulting PDF based on the standard deviation of this nearby set and returns a single Gaussian with a mean and width defined as such.<br>\n",
                 "\n",
-                "The current version of the code consists of a training stage, `Inform_CMNNPDF`, that computes colors for a set of training data (replacing non-detections with the 1-sigma limiting magnitude), and an estimation stage `CMNNPDF` that calculates the Mahalanobis distance to each training galaxy for each test galaxy and returns a single Guassian PDF for each galaxy where the mean can be estimated in one of three ways (see selection mode below), and the width is determined by the standard deviation of training galaxy redshifts within the threshold Mahalanobis distance. Future implementation improvements may change the output format to include multiple Gaussians.\n",
+                "The current version of the code consists of a training stage, `Inform_CMNNPDF`, that computes colors for a set of training data and an estimation stage `CMNNPDF` that calculates the Mahalanobis distance to each training galaxy for each test galaxy and returns a single Guassian PDF for each galaxy.   The mean value of this Gaussian PDF can be estimated in one of three ways (see selection mode below), and the width is determined by the standard deviation of training galaxy redshifts within the threshold Mahalanobis distance. Future implementation improvements may change the output format to include multiple Gaussians.\n",
+                "\n",
+                "For the color calculation, there is an option for how to treat the \"non-detections\" in a band: the default choice is to ignore any colors that contain a non-detect magnitude and adjust the number of degrees of freedom in the Mahalanobis distance accordingly (this is how the CMNN algorithm was originally implemented).  Or, if the configuration parameter `nondetect_replace` is set to `True` in `Inform_CMNNPDF`, the non-detected magnitudes will be replaced with the 1-sigma limiting magnitude in each band as supplied by the user via the `mag_limits` configuration parameter (or by the default 1-sigma limits if the user does not supply specific numbers).  We have not done any exploration of the relative performance of these two choices, but note that there is not a significant performance difference in terms of runtime between the two methods.<br>\n",
                 "\n",
                 "In addition to the Gaussian PDF for each test galaxy, two ancillary quantities are stored: `zmode`: the mode of the redshift PDF and `Ncm`, the integer number of \"nearby\" galaxies considered as neighbors for each galaxy.<br>\n",
                 "\n",
                 "`Inform_CMNNPDF` takes in a training data set and returns a model file that simply consists of the computed colors and color errors (magnitude errors added in quadrature) for that dataset, the model to be used in the `CMNNPDF` stage. A modification of the original CMNN algorithm, \"nondetections\" are now replaced by the 1-sigma limiting magnitudes and the non-detect magnitude errors replaced with a value of 1.0. The config parameters that can be set by the user for `Inform_CMNNPDF` are:\n",
                 "\n",
                 "- bands: list of the band names that should be present in the input data.<br>\n",
                 "- err_bands: list of the magnitude error column names that should be present in the input data.<br>\n",
                 "- redshift_col: a string giving the name for the redshift column present in the input data.<br>\n",
                 "- mag_limits: a dictionary with keys that match those in bands and a float with the 1 sigma limiting magnitude for each band.<br>\n",
                 "- nondetect_val: float or np.nan, the value indicating a non-detection, which will be replaced by the values in mag_limits.<br>\n",
+                "- nondetect_replace: bool, if set to `False` (the default) this option ignores colors with non-detected values in the Mahalanobis distance calculation, with a corresponding drop in the degrees of freedom value.  If set to `True`, the method will replace non-detections with the 1-sigma limiting magnitudes specified via `mag_limits` (or default 1-sigma limits if not supplied), and will use all colors in the Mahalanobis distance calculation.<br>\n",
                 "\n",
                 "\n",
                 "The parameters that can be set via the config_params in `CMNNPDF` are described in brief below:\n",
                 "\n",
                 "- bands, err_bands, redshift_col, mag_limits are all the same as described above for Inform_CMNNPDF.\n",
                 "- ppf_value: float, usually 0.68 or 0.95, which sets the value of the PPF used in the Mahalanobis distance calculation.\n",
                 "- selection_mode: int, selects how the central value of the Gaussian PDF is calculated in the algorithm, if set to **0** randomly chooses from set within the Mahalanobis distance, if set to **1** chooses the nearest neighbor point, if set to **2** adds a distance weight to the random choice.\n",
@@ -155,15 +158,15 @@
                 "pz_train.inform(training_data)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "We can now set up the main photo-z stage and run our algorithm on the data to produce simple photo-z estimates.  Note that we are loading the trained model that we computed from the inform stage: with the `model=pz_train.get_handle('model')` statement.<br>\n",
+                "We can now set up the main photo-z stage and run our algorithm on the data to produce simple photo-z estimates.  Note that we are loading the trained model that we computed from the inform stage: with the `model=pz_train.get_handle('model')` statement.  We will set `nondetect_replace` to `True` to replace our non-detection magnitudes with their 1-sigma limits and use all colors.<br>\n",
                 "\n",
                 "Let's also set the minumum number of neighbors to 24, and the `selection_mode` to \"1\", which will choose the nearest neighbor for each galaxy as the redshift estimate:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -171,14 +174,15 @@
             "outputs": [],
             "source": [
                 "%%time\n",
                 "pz = CMNNPDF.make_stage(name='CMNN', hdf5_groupname='photometry',\n",
                 "                        model=pz_train.get_handle('model'),\n",
                 "                        min_n=20,\n",
                 "                        selection_mode=1,\n",
+                "                        nondetect_replace=True,\n",
                 "                        aliases={\"output\":\"pz_near\"})\n",
                 "results = pz.estimate(test_data)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -248,14 +252,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "pz_rand = CMNNPDF.make_stage(name='CMNN_rand', hdf5_groupname='photometry',\n",
                 "                             model=pz_train.get_handle('model'),\n",
                 "                             min_n=20,\n",
                 "                             selection_mode=0,\n",
+                "                             nondetect_replace=True,\n",
                 "                             aliaes={\"output\": \"pz_rand\"})\n",
                 "results_rand = pz_rand.estimate(test_data)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -284,14 +289,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "pz_weight = CMNNPDF.make_stage(name='CMNN_weight', hdf5_groupname='photometry',\n",
                 "                               model=pz_train.get_handle('model'),\n",
                 "                               min_n=20,\n",
                 "                               selection_mode=2,\n",
+                "                               nondetect_replace=True,\n",
                 "                               aliaes={\"output\": \"pz_weight\"})\n",
                 "results_weight = pz_weight.estimate(test_data)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
```

### Comparing `pz-rail-cmnn-0.0.2/pyproject.toml` & `pz-rail-cmnn-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pz-rail-cmnn-0.0.2/src/pz_rail_cmnn.egg-info/PKG-INFO` & `pz-rail-cmnn-0.1.0/src/pz_rail_cmnn.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-cmnn
-Version: 0.0.2
+Version: 0.1.0
 Summary: RAIL CMNN Interface
 Author-email: The LSST DESC PZ WG <samuel.j.schmidt@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,22 +43,25 @@
 RAIL interface to Melissa Graham's CMNN algorithm.  A slight modification of the original code found here: <br>
 [dirac-institute/CMNN_Photoz_estimator](https://github.com/dirac-institute/CMNN_Photoz_Estimator)
 
 See https://ui.adsabs.harvard.edu/abs/2018AJ....155....1G/abstract
 for more details on the code
 Any use of `rail_cmnn` in a paper or report should cite [Graham et al. (2018)](https://ui.adsabs.harvard.edu/abs/2018AJ....155....1G/abstract).
 
-The current version of the code consists of a training stage, `Inform_CMNNPDF`, that computes colors for a set of training data (replacing non-detections with the 1-sigma limiting magnitude), and an estimation stage `CMNNPDF` that calculates the Mahalanobis distance to each training galaxy for each test galaxy and returns a single Guassian PDF for each galaxy where the mean can be estimated in one of three ways (see `selection mode` below), and the width is determined by the standard deviation of training galaxy redshifts within the threshold Mahalanobis distance.  Future implementation improvements may change the output format to include multiple Gaussians.
+The current version of the code consists of a training stage, `Inform_CMNNPDF`, that computes colors for a set of training data and an estimation stage `CMNNPDF` that calculates the Mahalanobis distance to each training galaxy for each test galaxy. The mean value of this Guassian PDF can be estimated in one of three ways (see `selection mode` below), and the width is determined by the standard deviation of training galaxy redshifts within the threshold Mahalanobis distance.  Future implementation improvements may change the output format to include multiple Gaussians.
+
+For the color calculation, there is an option for how to treat the "non-detections" in a band: the default choice is to ignore any colors that contain a non-detect magnitude and adjust the number of degrees of freedom in the Mahalanobis distance accordingly (this is how the CMNN algorithm was originally implemented). Or, if the configuration parameter `nondetect_replace` is set to `True` in `Inform_CMNNPDF`, the non-detected magnitudes will be replaced with the 1-sigma limiting magnitude in each band as supplied by the user via the `mag_limits` configuration parameter (or by the default 1-sigma limits if the user does not supply specific numbers). We have not done any exploration of the relative performance of these two choices, but note that there is not a significant performance difference in terms of runtime between the two methods.
 
 `Inform_CMNNPDF` takes in a training data set and returns a model file that simply consists of the computed colors and color errors (magnitude errors added in quadrature) for that dataset, the model to be used in the `CMNNPDF` stage. A modification of the original CMNN algorithm, "nondetections" are now replaced by the 1-sigma limiting magnitudes and the non-detect magnitude errors replaced with a value of 1.0.  The config parameters that can be set by the user for `Inform_CMNNPDF` are:<br>
 - `bands`: list of the band names that should be present in the input data.<br>
 - `err_bands`: list of the magnitude error column names that should be present in the input data.<br>
 - `redshift_col`: a string giving the name for the redshift column present in the input data.<br>
 - `mag_limits`: a dictionary with keys that match those in `bands` and a float with the 1 sigma limiting magnitude for each band.<br>
 - nondetect_val: float or `np.nan`, the value indicating a non-detection, which will be replaced by the values in `mag_limits`.<br>
+- `nondetect_replace`: bool, if set to False (the default) this option ignores colors with non-detected values in the Mahalanobis distance calculation, with a corresponding drop in the degrees of freedom value. If set to True, the method will replace non-detections with the 1-sigma limiting magnitudes specified via `mag_limits` (or default 1-sigma limits if not supplied), and will use all colors in the Mahalanobis distance calculation.
 
 
 The parameters that can be set via the `config_params` in `CMNNPDF` are described in brief below:<br>
 - `bands`, `err_bands`, `redshift_col`, `mag_limits` are all the same as described above for `Inform_CMNNPDF.`<br>
 - `ppf_value`: float, usually 0.68 or 0.95, which sets the value of the PPF used in the Mahalanobis distance calculation.<br>
 - `selection_mode`: int, selects how the central value of the Gaussian PDF is calculated in the algorithm, if set to `0` randomly chooses from set within the Mahalanobis distance, if set to `1` chooses the nearest neighbor point, if set to `2` adds a distance weight to the random choice.<br>
 - `min_n`: int, the minimum number of training galaxies to use.<br>
```

### Comparing `pz-rail-cmnn-0.0.2/src/rail/estimation/algos/cmnn.py` & `pz-rail-cmnn-0.1.0/src/rail/estimation/algos/cmnn.py`

 * *Files 15% similar despite different names*

```diff
@@ -36,44 +36,51 @@
     """
     name = 'Inform_CMNNPDF'
     config_options = CatInformer.config_options.copy()
     config_options.update(bands=SHARED_PARAMS,
                           err_bands=SHARED_PARAMS,
                           redshift_col=SHARED_PARAMS,
                           mag_limits=SHARED_PARAMS,
-                          nondetect_val=SHARED_PARAMS)
+                          nondetect_val=SHARED_PARAMS,
+                          nondetect_replace=Param(bool, False, msg="set to True to replace non-detects,"
+                                                  " False to ignore in distance calculation"))
 
     def __init__(self, args, comm=None):
         """ Constructor
         Do CatInformer specific initialization, then check on bands """
         CatInformer.__init__(self, args, comm=comm)
 
     def run(self):
         if self.config.hdf5_groupname:
             training_data = self.get_data('input')[self.config.hdf5_groupname]
-        else:  #pragma: no cover
+        else:  # pragma: no cover
             training_data = self.get_data('input')
         specz = np.array(training_data[self.config['redshift_col']])
 
         # replace nondetects
-        for col,err in zip(self.config.bands, self.config.err_bands):
+        for col, err in zip(self.config.bands, self.config.err_bands):
             if np.isnan(self.config.nondetect_val):  # pragma: no cover
                 mask = np.isnan(training_data[col])
             else:
                 mask = np.isclose(training_data[col], self.config.nondetect_val)
-            training_data[col][mask] = self.config.mag_limits[col]
-            training_data[err][mask] = 1.0  # could also put 0.757 for 1 sigma, but slightly inflated seems good
+            if self.config.nondetect_replace:
+                training_data[col][mask] = self.config.mag_limits[col]
+                training_data[err][mask] = 1.0  # could also put 0.757 for 1 sigma, but slightly inflated seems good
+            else:
+                training_data[col][mask] = np.nan
+                training_data[err][mask] = np.nan
 
         col_data, col_err = _computecolordata(training_data,
                                               self.config.bands,
                                               self.config.err_bands)
 
-        self.model = dict(train_color=col_data, train_err=col_err, truez=specz)
+        self.model = dict(train_color=col_data, train_err=col_err, truez=specz,
+                          nondet_choice=self.config.nondetect_replace)
         self.add_data('model', self.model)
-        
+
 
 class CMNNPDF(CatEstimator):
     """Color Matched Nearest Neighbor Estimator
     Note that there are several modifications from the original CMNN, mainly that
     the original estimator dropped non-detections from the Mahalnobis distance
     calculation. However, there is information in a non-detection, so instead here
     I've replaced the non-detections with 1 sigma limit and a magnitude
@@ -104,15 +111,15 @@
                           bands=SHARED_PARAMS,
                           err_bands=SHARED_PARAMS,
                           nondetect_val=SHARED_PARAMS,
                           mag_limits=SHARED_PARAMS,
                           redshift_col=SHARED_PARAMS,
                           seed=Param(int, 66, msg="random seed used in selection mode"),
                           ppf_value=Param(float, 0.68, msg="PPF value used in Mahalanobis distance"),
-                          selection_mode=Param(int, 1, msg="select which mode to choose the redshift estimate:" +
+                          selection_mode=Param(int, 1, msg="select which mode to choose the redshift estimate:"
                                                "0: randomly choose, 1: nearest neigh, 2: weighted random"),
                           min_n=Param(int, 25, msg="minimum number of training galaxies to use"),
                           min_thresh=Param(float, 0.0001, msg="minimum threshold cutoff"),
                           min_dist=Param(float, 0.0001, msg="minimum Mahalanobis distance"),
                           bad_redshift_val=Param(float, 99., msg="redshift to assign bad redshifts"),
                           bad_redshift_err=Param(float, 10., msg="Gauss error width to assign to bad redshifts")
                           )
@@ -131,47 +138,70 @@
     def open_model(self, **kwargs):
         CatEstimator.open_model(self, **kwargs)
         if self.model is None:  # pragma: no cover
             return
         self.train_color = self.model['train_color']
         self.train_err = self.model['train_err']
         self.truez = self.model['truez']
+        self.nondet_choice = self.model['nondet_choice']
 
     def _process_chunk(self, start, end, data, first):
         print(f"Process {self.rank} estimating PZ PDF for rows {start:,} - {end:,}")
         # replace nondetects
-        for col,err in zip(self.config.bands, self.config.err_bands):
+        for col, err in zip(self.config.bands, self.config.err_bands):
             if np.isnan(self.config.nondetect_val):  # pragma: no cover
                 mask = np.isnan(data[col])
             else:
                 mask = np.isclose(data[col], self.config.nondetect_val)
-            data[col][mask] = self.config.mag_limits[col]
-            data[err][mask] = 1.0  # could also put 0.757 for 1 sigma, but slightly inflated seems good
-        
+            if self.nondet_choice:
+                data[col][mask] = self.config.mag_limits[col]
+                data[err][mask] = 1.0  # could also put 0.757 for 1 sigma, but slightly inflated seems good
+            else:
+                data[col][mask] = np.nan
+                data[err][mask] = np.nan
+
         test_color, test_err = _computecolordata(data,
                                                  self.config.bands,
                                                  self.config.err_bands)
         num_gals = test_color.shape[0]
+        ncols = test_color.shape[1]
+        # chi2.ppf calculation is slow and repeated a bunch if nondet_choice is false
+        # so precompute the potential values here and put in a lookup table
+        thresh_table = np.zeros(ncols + 1)
+        thresh_table[0] = 0.0  # this will never be used, just put in a zero
+        for ii in range(1, ncols + 1):
+            thresh_table[ii] = chi2.ppf(self.config.ppf_value, float(ii))
         chunk_pz = np.zeros(num_gals)
         chunk_pze = np.zeros(num_gals)
         chunk_ncm = np.zeros(num_gals, dtype=int)
-        rng = np.random.default_rng(seed = self.config.seed + start)
+        chunk_colused = np.zeros(num_gals, dtype=int)
+        rng = np.random.default_rng(seed=self.config.seed + start)
         for ii in range(num_gals):
-
             MahalanobisDistance = np.nansum((test_color[ii] - self.train_color)**2 / test_err[ii]**2, axis=1, dtype='float')
             # original CMNN algorithm determines degrees of freedom in a roundabout way that takes into account
             # non-detect bands.  I think with the replacement of non-detects with 1 sigma limit and large error
             # we should be ok to set this to just be num_bands - 1
-            deg_of_freedom = len(self.config.bands) - 1
-            threshold = chi2.ppf(self.config.ppf_value, deg_of_freedom)
-
+            if self.nondet_choice:
+                deg_of_freedom = len(self.config.bands) - 1
+                threshold = chi2.ppf(self.config.ppf_value, deg_of_freedom)
+                chunk_colused[ii] = deg_of_freedom
+            else:
+                doftest = ~np.isnan(test_color[ii])
+                deg_of_freedom = np.nansum((test_color[ii]**2 + self.train_color**2 + 1.0) / (test_color[ii]**2 + self.train_color**2 + 1.0),
+                                           axis=1, dtype='int')
+                ntrain = len(deg_of_freedom)
+                # this is the slow way to do things, comment out and replace!
+                # threshold = np.array([chi2.ppf(self.config.ppf_value, deg_of_freedom[xx]) for xx in range(ntrain)])
+                # lookup table-based way to get thresholds
+                threshold = np.array([thresh_table[deg_of_freedom[xx]] for xx in range(ntrain)])
+                chunk_colused[ii] = np.sum(doftest)
             # find the indices of galaxies meeting CMNN subset criteria
-            index = np.where((threshold > self.config.min_thresh) & \
-                             (MahalanobisDistance > self.config.min_dist) & \
-                             (MahalanobisDistance <= threshold) )[0]
+            index = np.where((threshold > self.config.min_thresh) &
+                             (MahalanobisDistance > self.config.min_dist) &
+                             (MahalanobisDistance <= threshold))[0]
 
             if len(index) >= self.config.min_n:
 
                 # choose randomly from the color matched sample
                 if self.config.selection_mode == 0:
                     rival = rng.choice(index, size=1, replace=False)[0]
                     out_pz = self.truez[rival]
@@ -184,15 +214,15 @@
                     if len(tx) == 1:
                         rval = tx[0]
                     if len(tx) > 1:  # pragma: no cover
                         # if there's more than one best match (rare but possible), choose randomly
                         rval = rng.choice(tx, size=1, replace=False)[0]
                     out_pz = self.truez[index[rval]]
                     out_pze = np.std(self.truez[index])
-                    del tx,rval
+                    del tx, rval
 
                 # weight by how good the color match is and then choose randomly
                 if self.config.selection_mode == 2:
                     tweights = float(1.00) / MahalanobisDistance[index]
                     weights = tweights / np.sum(tweights)
                     rival = rng.choice(index, size=1, replace=False, p=weights)[0]
                     out_pz = self.truez[rival]
@@ -206,40 +236,47 @@
                     tempMD = MahalanobisDistance[index2]
                     tempTZ = self.truez[index2]
                     # identify the nearest neighbors and use them as the CMNN subset
                     # create a sorted list of min_Nn
                     sx = np.argsort(tempMD)
                     new_MD = np.asarray(tempMD[sx[0:self.config.min_n]], dtype='float')
                     new_TZ = np.asarray(tempTZ[sx[0:self.config.min_n]], dtype='float')
+                    if self.nondet_choice:
+                        lim_DOF = deg_of_freedom
+                    else:
+                        tmpDOF = deg_of_freedom[index2]
+                        new_DOF = np.asarray(tmpDOF[sx[0:self.config.min_n]], dtype='float')
+                        lim_DOF = new_DOF[-1]
+                        del new_DOF
                     del tempMD, tempTZ, sx
-                    ### calculate the new 'effective PPF' based on the most distant nearest neighbor
-                    new_ppf_value = chi2.cdf(new_MD[-1], deg_of_freedom)
-                    ### inflate the photo-z error appropriately
-                    temp = np.std( new_TZ )
+                    # calculate the new 'effective PPF' based on the most distant nearest neighbor
+                    new_ppf_value = chi2.cdf(new_MD[-1], lim_DOF)
+                    # inflate the photo-z error appropriately
+                    temp = np.std(new_TZ)
                     out_pze = temp * (new_ppf_value / self.config.ppf_value)
-                    del temp,new_ppf_value
+                    del temp, new_ppf_value
                     if self.config.selection_mode == 0:
                         rval = rng.choice(self.config.min_n, size=1, replace=False)[0]
                         out_pz = new_TZ[rval]
                         del rval
                     if self.config.selection_mode == 1:
                         out_pz = new_TZ[0]
                     if self.config.selection_mode == 2:
                         tweights = float(1.00) / new_MD
                         weights = tweights / np.sum(tweights)
                         cx = rng.choice(self.config.min_n, size=1, replace=False, p=weights)[0]
                         out_pz = new_TZ[cx]
                         del tweights, weights, cx
-                    del new_MD,new_TZ
+                    del new_MD, new_TZ
                     Ncm = self.config.min_n
                 else:  # pragma: no cover
                     # I think this would only happen if there are less than min_n gals in training set
                     out_pz = self.config.bad_redshift_val
                     out_pze = self.config.bad_redshift_err
                     Ncm = 0
             chunk_pz[ii] = out_pz
             chunk_pze[ii] = out_pze
             chunk_ncm[ii] = Ncm
         ens = qp.Ensemble(qp.stats.norm, data=dict(loc=np.expand_dims(chunk_pz, -1),
                                                    scale=np.expand_dims(chunk_pze, -1)))
-        ens.set_ancil(dict(zmode=chunk_pz, Ncm=chunk_ncm))
+        ens.set_ancil(dict(ncolors=chunk_colused, zmode=chunk_pz, Ncm=chunk_ncm))
         self._do_chunk_output(ens, start, end, first)
```

### Comparing `pz-rail-cmnn-0.0.2/tests/test_algos.py~` & `pz-rail-cmnn-0.1.0/tests/test_algos.py~`

 * *Files identical despite different names*

