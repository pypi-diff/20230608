# Comparing `tmp/xarray-safe-s1-2023.6.1.tar.gz` & `tmp/xarray-safe-s1-2023.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xarray-safe-s1-2023.6.1.tar", last modified: Thu Jun  8 09:28:24 2023, max compression
+gzip compressed data, was "xarray-safe-s1-2023.6.2.tar", last modified: Fri Jun  2 08:50:18 2023, max compression
```

## Comparing `xarray-safe-s1-2023.6.1.tar` & `xarray-safe-s1-2023.6.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:28:24.543736 xarray-safe-s1-2023.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-08 09:28:06.000000 xarray-safe-s1-2023.6.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:28:24.539736 xarray-safe-s1-2023.6.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-08 09:28:06.000000 xarray-safe-s1-2023.6.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:28:24.539736 xarray-safe-s1-2023.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-08 09:28:06.000000 xarray-safe-s1-2023.6.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-08 09:28:06.000000 xarray-safe-s1-2023.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-08 09:28:06.000000 xarray-safe-s1-2023.6.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-08 09:28:06.000000 xarray-safe-s1-2023.6.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-08 09:28:06.000000 xarray-safe-s1-2023.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-06-08 09:28:24.543736 xarray-safe-s1-2023.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7423 2023-06-08 09:28:06.000000 xarray-safe-s1-2023.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:28:24.539736 xarray-safe-s1-2023.6.1/ci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:28:24.539736 xarray-safe-s1-2023.6.1/ci/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-08 09:28:06.000000 xarray-safe-s1-2023.6.1/ci/requirements/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-08 09:28:06.000000 xarray-safe-s1-2023.6.1/ci/requirements/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:28:24.543736 xarray-safe-s1-2023.6.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-08 09:28:06.000000 xarray-safe-s1-2023.6.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:28:24.539736 xarray-safe-s1-2023.6.1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:28:24.543736 xarray-safe-s1-2023.6.1/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-08 09:28:06.000000 xarray-safe-s1-2023.6.1/docs/_static/css/xsar.css
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-08 09:28:06.000000 xarray-safe-s1-2023.6.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-06-08 09:28:06.000000 xarray-safe-s1-2023.6.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:28:24.543736 xarray-safe-s1-2023.6.1/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-06-08 09:28:06.000000 xarray-safe-s1-2023.6.1/docs/examples/simple_tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-08 09:28:06.000000 xarray-safe-s1-2023.6.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-08 09:28:06.000000 xarray-safe-s1-2023.6.1/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-08 09:28:06.000000 xarray-safe-s1-2023.6.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-08 09:28:06.000000 xarray-safe-s1-2023.6.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-08 09:28:06.000000 xarray-safe-s1-2023.6.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:28:24.543736 xarray-safe-s1-2023.6.1/safe_s1/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-08 09:28:06.000000 xarray-safe-s1-2023.6.1/safe_s1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-08 09:28:06.000000 xarray-safe-s1-2023.6.1/safe_s1/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)    27954 2023-06-08 09:28:06.000000 xarray-safe-s1-2023.6.1/safe_s1/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    42087 2023-06-08 09:28:06.000000 xarray-safe-s1-2023.6.1/safe_s1/sentinel1_xml_mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-06-08 09:28:06.000000 xarray-safe-s1-2023.6.1/safe_s1/xml_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 09:28:24.543736 xarray-safe-s1-2023.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:28:24.543736 xarray-safe-s1-2023.6.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-08 09:28:06.000000 xarray-safe-s1-2023.6.1/test/test_s1reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:28:24.543736 xarray-safe-s1-2023.6.1/xarray_safe_s1.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-06-08 09:28:24.000000 xarray-safe-s1-2023.6.1/xarray_safe_s1.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-08 09:28:24.000000 xarray-safe-s1-2023.6.1/xarray_safe_s1.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 09:28:24.000000 xarray-safe-s1-2023.6.1/xarray_safe_s1.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-08 09:28:24.000000 xarray-safe-s1-2023.6.1/xarray_safe_s1.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-08 09:28:24.000000 xarray-safe-s1-2023.6.1/xarray_safe_s1.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:50:18.356232 xarray-safe-s1-2023.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:50:18.352232 xarray-safe-s1-2023.6.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:50:18.352232 xarray-safe-s1-2023.6.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-06-02 08:50:18.356232 xarray-safe-s1-2023.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7423 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:50:18.352232 xarray-safe-s1-2023.6.2/ci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:50:18.352232 xarray-safe-s1-2023.6.2/ci/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/ci/requirements/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/ci/requirements/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:50:18.356232 xarray-safe-s1-2023.6.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:50:18.352232 xarray-safe-s1-2023.6.2/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:50:18.356232 xarray-safe-s1-2023.6.2/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/docs/_static/css/xsar.css
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:50:18.356232 xarray-safe-s1-2023.6.2/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/docs/examples/simple_tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:50:18.356232 xarray-safe-s1-2023.6.2/safe_s1/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/safe_s1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/safe_s1/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    27910 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/safe_s1/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42062 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/safe_s1/sentinel1_xml_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/safe_s1/xml_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 08:50:18.356232 xarray-safe-s1-2023.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:50:18.356232 xarray-safe-s1-2023.6.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/test/test_s1reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:50:18.356232 xarray-safe-s1-2023.6.2/xarray_safe_s1.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-06-02 08:50:18.000000 xarray-safe-s1-2023.6.2/xarray_safe_s1.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-02 08:50:18.000000 xarray-safe-s1-2023.6.2/xarray_safe_s1.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 08:50:18.000000 xarray-safe-s1-2023.6.2/xarray_safe_s1.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-02 08:50:18.000000 xarray-safe-s1-2023.6.2/xarray_safe_s1.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 08:50:18.000000 xarray-safe-s1-2023.6.2/xarray_safe_s1.egg-info/top_level.txt
```

### Comparing `xarray-safe-s1-2023.6.1/.github/workflows/publish.yml` & `xarray-safe-s1-2023.6.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2023.6.1/.pre-commit-config.yaml` & `xarray-safe-s1-2023.6.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2023.6.1/LICENSE` & `xarray-safe-s1-2023.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2023.6.1/PKG-INFO` & `xarray-safe-s1-2023.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xarray-safe-s1
-Version: 2023.6.1
+Version: 2023.6.2
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 [![Documentation Status](https://readthedocs.org/projects/xarray-safe-s1/badge/?version=latest)](https://xarray-safe-s1.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `xarray-safe-s1-2023.6.1/README.md` & `xarray-safe-s1-2023.6.2/README.md`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2023.6.1/ci/requirements/environment.yaml` & `xarray-safe-s1-2023.6.2/ci/requirements/environment.yaml`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2023.6.1/docs/Makefile` & `xarray-safe-s1-2023.6.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2023.6.1/docs/conf.py` & `xarray-safe-s1-2023.6.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2023.6.1/docs/examples/simple_tutorial.ipynb` & `xarray-safe-s1-2023.6.2/docs/examples/simple_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2023.6.1/docs/index.rst` & `xarray-safe-s1-2023.6.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2023.6.1/docs/installing.rst` & `xarray-safe-s1-2023.6.2/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2023.6.1/docs/make.bat` & `xarray-safe-s1-2023.6.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2023.6.1/pyproject.toml` & `xarray-safe-s1-2023.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2023.6.1/safe_s1/metadata.py` & `xarray-safe-s1-2023.6.2/safe_s1/metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,14 @@
                 'doppler_estimate': self.doppler_estimate,
                 'bursts': self.bursts,
                 'calibration_luts': self.get_calibration_luts,
                 'noise_azimuth_raw': self.get_noise_azi_raw,
                 'noise_range_raw': self.get_noise_range_raw,
             }
             self.dt = datatree.DataTree.from_dict(self._dict)
-            assert self.dt==self.datatree
 
     def load_digital_number(self, resolution=None, chunks=None, resampling=rasterio.enums.Resampling.rms):
         """
         load digital_number from self.sar_meta.files['measurement'], as an `xarray.Dataset`.
 
         Parameters
         ----------
@@ -576,15 +575,15 @@
         """
         tmp = []
         pols = []
         history = []
         for pol_code, xml_file in self.files['noise'].items():
             pol = os.path.basename(xml_file).split('-')[4].upper()
             pols.append(pol)
-            if self.product == 'SLC' or self.product == 'SL2':
+            if self.product == 'SLC' or self.product=='SL2':
                 noise_lut_azi_raw_ds = self.xml_parser.get_compound_var(xml_file, 'noise_lut_azi_raw_slc')
                 history.append(self.xml_parser.get_compound_var(xml_file, 'noise_lut_azi_raw_slc', describe=True))
             else:
                 noise_lut_azi_raw_ds = self.xml_parser.get_compound_var(xml_file, 'noise_lut_azi_raw_grd')
                 #noise_lut_azi_raw_ds.attrs[f'raw_azi_lut_{pol}'] = \
                 #    self.xml_parser.get_var(xml_file, 'noise.azi.noiseLut')
                 history.append(self.xml_parser.get_compound_var(xml_file, 'noise_lut_azi_raw_grd', describe=True))
```

### Comparing `xarray-safe-s1-2023.6.1/safe_s1/sentinel1_xml_mappings.py` & `xarray-safe-s1-2023.6.2/safe_s1/sentinel1_xml_mappings.py`

 * *Files 0% similar despite different names*

```diff
@@ -535,15 +535,15 @@
     radar_frequency: float [second-1]
     range_sampling_rate: float
     azimuth_steering_rate: float
     Returns
     -------
     xarray.Dataset
     """
-    if product_type == 'SLC' or product_type == 'SL2':
+    if product_type == 'SLC':
         pixel_sample_m = rangePixelSpacing / np.sin(np.radians(incidence_angle_mid_swath))
     else:
         pixel_sample_m = rangePixelSpacing
     tmp = {
         'LineUtcTime': (line_time_range, 'line_time_range'),
         'numberOfLines': (line_size, 'line_size'),
         'numberOfSamples': (sample_size, 'sample_size'),
```

### Comparing `xarray-safe-s1-2023.6.1/safe_s1/xml_parser.py` & `xarray-safe-s1-2023.6.2/safe_s1/xml_parser.py`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2023.6.1/test/test_s1reader.py` & `xarray-safe-s1-2023.6.2/test/test_s1reader.py`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2023.6.1/xarray_safe_s1.egg-info/PKG-INFO` & `xarray-safe-s1-2023.6.2/xarray_safe_s1.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xarray-safe-s1
-Version: 2023.6.1
+Version: 2023.6.2
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 [![Documentation Status](https://readthedocs.org/projects/xarray-safe-s1/badge/?version=latest)](https://xarray-safe-s1.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `xarray-safe-s1-2023.6.1/xarray_safe_s1.egg-info/SOURCES.txt` & `xarray-safe-s1-2023.6.2/xarray_safe_s1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

