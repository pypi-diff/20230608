# Comparing `tmp/sdcpy-0.2.0.tar.gz` & `tmp/sdcpy-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdcpy-0.2.0.tar", last modified: Tue Jan 19 12:28:36 2021, max compression
+gzip compressed data, was "sdcpy-0.2.2.tar", last modified: Mon Feb 15 13:47:43 2021, max compression
```

## Comparing `sdcpy-0.2.0.tar` & `sdcpy-0.2.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-19 12:28:36.913195 sdcpy-0.2.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)      169 2021-01-19 12:25:38.000000 sdcpy-0.2.0/AUTHORS.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     3485 2021-01-19 12:25:38.000000 sdcpy-0.2.0/CONTRIBUTING.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       89 2021-01-19 12:25:38.000000 sdcpy-0.2.0/HISTORY.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1075 2021-01-19 12:25:38.000000 sdcpy-0.2.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      262 2021-01-19 12:25:38.000000 sdcpy-0.2.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     2408 2021-01-19 12:28:36.913195 sdcpy-0.2.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1329 2021-01-19 12:25:38.000000 sdcpy-0.2.0/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-19 12:28:36.909196 sdcpy-0.2.0/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)      606 2021-01-19 12:25:38.000000 sdcpy-0.2.0/docs/Makefile
--rw-rw-r--   0 travis    (2000) travis    (2000)       28 2021-01-19 12:25:38.000000 sdcpy-0.2.0/docs/authors.rst
--rwxrwxr-x   0 travis    (2000) travis    (2000)     4795 2021-01-19 12:25:38.000000 sdcpy-0.2.0/docs/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       33 2021-01-19 12:25:38.000000 sdcpy-0.2.0/docs/contributing.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       28 2021-01-19 12:25:38.000000 sdcpy-0.2.0/docs/history.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      302 2021-01-19 12:25:38.000000 sdcpy-0.2.0/docs/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1098 2021-01-19 12:25:38.000000 sdcpy-0.2.0/docs/installation.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      803 2021-01-19 12:25:38.000000 sdcpy-0.2.0/docs/make.bat
--rw-rw-r--   0 travis    (2000) travis    (2000)       27 2021-01-19 12:25:38.000000 sdcpy-0.2.0/docs/readme.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       65 2021-01-19 12:25:38.000000 sdcpy-0.2.0/docs/usage.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      100 2021-01-19 12:27:02.000000 sdcpy-0.2.0/pyproject.toml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-19 12:28:36.909196 sdcpy-0.2.0/sdcpy/
--rw-rw-r--   0 travis    (2000) travis    (2000)      161 2021-01-19 12:25:38.000000 sdcpy-0.2.0/sdcpy/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    25636 2021-01-19 12:25:38.000000 sdcpy-0.2.0/sdcpy/scale_dependent_correlation.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-19 12:28:36.913195 sdcpy-0.2.0/sdcpy.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2408 2021-01-19 12:28:36.000000 sdcpy-0.2.0/sdcpy.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      517 2021-01-19 12:28:36.000000 sdcpy-0.2.0/sdcpy.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-01-19 12:28:36.000000 sdcpy-0.2.0/sdcpy.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-01-19 12:25:40.000000 sdcpy-0.2.0/sdcpy.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)       52 2021-01-19 12:28:36.000000 sdcpy-0.2.0/sdcpy.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        6 2021-01-19 12:28:36.000000 sdcpy-0.2.0/sdcpy.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      561 2021-01-19 12:28:36.913195 sdcpy-0.2.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1259 2021-01-19 12:25:38.000000 sdcpy-0.2.0/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-19 12:28:36.913195 sdcpy-0.2.0/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)      605 2021-01-19 12:25:38.000000 sdcpy-0.2.0/tests/test_sdcpy.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-15 13:47:43.016921 sdcpy-0.2.2/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      169 2021-02-15 13:44:57.000000 sdcpy-0.2.2/AUTHORS.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3485 2021-02-15 13:44:57.000000 sdcpy-0.2.2/CONTRIBUTING.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       89 2021-02-15 13:44:57.000000 sdcpy-0.2.2/HISTORY.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1075 2021-02-15 13:44:57.000000 sdcpy-0.2.2/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      262 2021-02-15 13:44:57.000000 sdcpy-0.2.2/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2681 2021-02-15 13:47:43.016921 sdcpy-0.2.2/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1599 2021-02-15 13:44:57.000000 sdcpy-0.2.2/README.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-15 13:47:43.016921 sdcpy-0.2.2/docs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      606 2021-02-15 13:44:57.000000 sdcpy-0.2.2/docs/Makefile
+-rw-rw-r--   0 travis    (2000) travis    (2000)       28 2021-02-15 13:44:57.000000 sdcpy-0.2.2/docs/authors.rst
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     4795 2021-02-15 13:44:57.000000 sdcpy-0.2.2/docs/conf.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       33 2021-02-15 13:44:57.000000 sdcpy-0.2.2/docs/contributing.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       28 2021-02-15 13:44:57.000000 sdcpy-0.2.2/docs/history.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      302 2021-02-15 13:44:57.000000 sdcpy-0.2.2/docs/index.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1098 2021-02-15 13:44:57.000000 sdcpy-0.2.2/docs/installation.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      803 2021-02-15 13:44:57.000000 sdcpy-0.2.2/docs/make.bat
+-rw-rw-r--   0 travis    (2000) travis    (2000)       27 2021-02-15 13:44:57.000000 sdcpy-0.2.2/docs/readme.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       65 2021-02-15 13:44:57.000000 sdcpy-0.2.2/docs/usage.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      100 2021-02-15 13:46:10.000000 sdcpy-0.2.2/pyproject.toml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-15 13:47:43.016921 sdcpy-0.2.2/sdcpy/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      161 2021-02-15 13:44:57.000000 sdcpy-0.2.2/sdcpy/__init__.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    26998 2021-02-15 13:44:57.000000 sdcpy-0.2.2/sdcpy/scale_dependent_correlation.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-15 13:47:43.016921 sdcpy-0.2.2/sdcpy.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2681 2021-02-15 13:47:42.000000 sdcpy-0.2.2/sdcpy.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      517 2021-02-15 13:47:42.000000 sdcpy-0.2.2/sdcpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-02-15 13:47:42.000000 sdcpy-0.2.2/sdcpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-02-15 13:44:59.000000 sdcpy-0.2.2/sdcpy.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)       52 2021-02-15 13:47:42.000000 sdcpy-0.2.2/sdcpy.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        6 2021-02-15 13:47:42.000000 sdcpy-0.2.2/sdcpy.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      561 2021-02-15 13:47:43.016921 sdcpy-0.2.2/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1246 2021-02-15 13:44:57.000000 sdcpy-0.2.2/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-15 13:47:43.016921 sdcpy-0.2.2/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      605 2021-02-15 13:44:57.000000 sdcpy-0.2.2/tests/test_sdcpy.py
```

### Comparing `sdcpy-0.2.0/CONTRIBUTING.rst` & `sdcpy-0.2.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `sdcpy-0.2.0/LICENSE` & `sdcpy-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sdcpy-0.2.0/PKG-INFO` & `sdcpy-0.2.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 1.1
 Name: sdcpy
-Version: 0.2.0
-Summary: Linear and non-linear Time Series Analysis methods.
+Version: 0.2.2
+Summary: Scale dependent correlation in Python.
 Home-page: https://github.com/AlFontal/sdcpy
 Author: Alejandro Fontal
 Author-email: alejandrofontal92@gmail.com
 License: MIT license
 Description: ======
         sdcpy
         ======
@@ -20,15 +20,15 @@
         .. image:: https://readthedocs.org/projects/sdcpy/badge/?version=latest
                 :target: https://sdcpy.readthedocs.io/en/latest/?badge=latest
                 :alt: Documentation Status
         
         
         
         
-        Scale Dependent Correlation (SDC) analysis [1, 2] in Python.
+        Scale Dependent Correlation (SDC) analysis [1, 2, 3] in Python.
         
         
         * Free software: MIT license
         * Documentation: https://sdcpy.readthedocs.io.
         
         
         Features
@@ -47,17 +47,19 @@
         ::
         
            pip install sdcpy
         
         References
         -----------
         
-        1. Rodríguez-Arias, Miquel Àngel, and Xavier Rodó. "A primer on the study of transitory dynamics in ecological series using the scale-dependent correlation analysis." Oecologia 138, no. 4 (2004): 485-504.
+        1. Rodó, X. (2001). Reversal of three global atmospheric fields linking changes in SST anomalies in the Pacific, Atlantic and Indian oceans at tropical latitudes and midlatitudes. ***Climate Dynamics***, 18:203-217. DOI: 10.1007/s003820100171.
         
-        2. Rodó, Xavier, and Miquel-Àngel Rodríguez-Arias. "A new method to detect transitory signatures and local time/space variability structures in the climate system: the scale-dependent correlation analysis." Climate Dynamics 27, no. 5 (2006): 441-458.
+        2. Rodríguez, M.A. & Rodó, X. (2004). A primer on the study of transitory dynamics in ecological series using the scale-dependent correlation analysis. ***Oecologia***, 138,485-504. DOI: 10.1007/s00442-003-1464-4.
+        
+        3. Rodó, X. & M.A. Rodriguez-Arias. (2006). A new method to detect transitory signatures and local time/space variability structures in the climate system: the scale-dependent correlation analysis. ***Climate Dynamics***, 27:441-458. DOI: 10.1007/s00382-005-0106-4.
         
         
         =======
         History
         =======
         
         0.1.0 (2020-10-09)
```

### Comparing `sdcpy-0.2.0/README.rst` & `sdcpy-0.2.2/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 .. image:: https://readthedocs.org/projects/sdcpy/badge/?version=latest
         :target: https://sdcpy.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 
 
 
 
-Scale Dependent Correlation (SDC) analysis [1, 2] in Python.
+Scale Dependent Correlation (SDC) analysis [1, 2, 3] in Python.
 
 
 * Free software: MIT license
 * Documentation: https://sdcpy.readthedocs.io.
 
 
 Features
@@ -39,10 +39,12 @@
 ::
 
    pip install sdcpy
 
 References
 -----------
 
-1. Rodríguez-Arias, Miquel Àngel, and Xavier Rodó. "A primer on the study of transitory dynamics in ecological series using the scale-dependent correlation analysis." Oecologia 138, no. 4 (2004): 485-504.
+1. Rodó, X. (2001). Reversal of three global atmospheric fields linking changes in SST anomalies in the Pacific, Atlantic and Indian oceans at tropical latitudes and midlatitudes. ***Climate Dynamics***, 18:203-217. DOI: 10.1007/s003820100171.
 
-2. Rodó, Xavier, and Miquel-Àngel Rodríguez-Arias. "A new method to detect transitory signatures and local time/space variability structures in the climate system: the scale-dependent correlation analysis." Climate Dynamics 27, no. 5 (2006): 441-458.
+2. Rodríguez, M.A. & Rodó, X. (2004). A primer on the study of transitory dynamics in ecological series using the scale-dependent correlation analysis. ***Oecologia***, 138,485-504. DOI: 10.1007/s00442-003-1464-4.
+
+3. Rodó, X. & M.A. Rodriguez-Arias. (2006). A new method to detect transitory signatures and local time/space variability structures in the climate system: the scale-dependent correlation analysis. ***Climate Dynamics***, 27:441-458. DOI: 10.1007/s00382-005-0106-4.
```

### Comparing `sdcpy-0.2.0/docs/Makefile` & `sdcpy-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sdcpy-0.2.0/docs/conf.py` & `sdcpy-0.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sdcpy-0.2.0/docs/installation.rst` & `sdcpy-0.2.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `sdcpy-0.2.0/docs/make.bat` & `sdcpy-0.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sdcpy-0.2.0/sdcpy/scale_dependent_correlation.py` & `sdcpy-0.2.2/sdcpy/scale_dependent_correlation.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 
 RECOGNIZED_METHODS = {
     'pearson': lambda x, y: stats.pearsonr(x, y),
     'spearman': lambda x, y: stats.spearmanr(x, y),
     'kendall': lambda x, y: stats.kendalltau(x, y),
 }
 
+CONSTANT_WARNING = {'pearson': stats.PearsonRConstantInputWarning,
+                    'spearman': stats.SpearmanRConstantInputWarning}
+
 
 def generate_correlation_map(x: np.ndarray, y: np.ndarray, method: str = 'pearson') -> np.ndarray:
     """
     Correlate each row in matrix X against each row in matrix Y.
 
     Parameters
     ----------
@@ -115,14 +118,15 @@
     -------
     pd.DataFrame
         Data frame with a row for each pair wise comparison containing information about the coordinates of each
         fragment used, the similarity obtained and the p-value from the randomised test.
     """
 
     method_fun = RECOGNIZED_METHODS[method] if method in RECOGNIZED_METHODS else method
+    # TODO: Proper calculation of number of iterations considering the range of lags selected
     n_iterations = (len(ts1) - fragment_size) * (len(ts2) - fragment_size)
     n_root = int(np.sqrt(n_permutations).round())
     sdc_array = np.empty(shape=(n_iterations, 7))
     sdc_array[:] = np.NaN
     i = 0
     progress_bar = tqdm(total=n_iterations, desc='Computing SDC', leave=False)
     # We iterate over all possible fragments of size `fragment_size` in both time-series
@@ -131,15 +135,18 @@
         for start_2 in range(len(ts2) - fragment_size):
             lag = start_1 - start_2
             if min_lag <= lag <= max_lag:
                 stop_2 = start_2 + fragment_size
                 fragment_1 = ts1[start_1: stop_1]
                 fragment_2 = ts2[start_2: stop_2]
                 # Compute the correlation/distance across both fragments
-                r, p_value = method_fun(fragment_1, fragment_2)
+                with warnings.catch_warnings():
+                    warnings.simplefilter("ignore")
+                    warnings.warn("Constant Fragment", CONSTANT_WARNING[method])
+                    r, p_value = method_fun(fragment_1, fragment_2)
                 if permutations:
                     # Randomize both fragments and compute their correlations.
                     if method.lower() in ['pearson', 'spearman']:
                         permuted_1 = shuffle_along_axis(np.tile(fragment_1, n_root).reshape(n_root, -1), axis=1)
                         permuted_2 = shuffle_along_axis(np.tile(fragment_2, n_root).reshape(n_root, -1), axis=1)
                         permuted_scores = generate_correlation_map(permuted_1, permuted_2, method=method).reshape(-1)
                     else:
@@ -149,19 +156,19 @@
                     # Get the p-value by comparing the original value to the distribution of randomized values
                     if two_tailed:
                         p_value = 1 - stats.percentileofscore(np.abs(permuted_scores), np.abs(r)) / 100
                     else:
                         p_value = 1 - stats.percentileofscore(permuted_scores, r) / 100
 
                 sdc_array[i] = [start_1, stop_1, start_2, stop_2, lag, r, p_value]
+                i += 1
             progress_bar.update(1)
-            i += 1
 
     progress_bar.close()
-    sdc_df = pd.DataFrame(sdc_array, columns=['start_1', 'stop_1', 'start_2', 'stop_2', 'lag', 'r', 'p_value'])
+    sdc_df = pd.DataFrame(sdc_array[:i], columns=['start_1', 'stop_1', 'start_2', 'stop_2', 'lag', 'r', 'p_value'])
 
     return sdc_df
 
 
 def plot_two_way_sdc(sdc_df: pd.DataFrame, alpha: float = .05, **kwargs):
     """
     Plots the results of a SDC analysis for a fixed window size in a 2D figure.
@@ -263,64 +270,83 @@
                           lag=lambda dd: dd.start_1 - dd.start_2)
                   .merge(ts1.reset_index()[['date_1', 'start_1']])
                   .merge(ts2.reset_index()[['date_2', 'start_2']]))
 
         return cls(ts1=ts1.ts1, ts2=ts2.ts2, fragment_size=fragment_size, n_permutations=n_permutations, method=method,
                    sdc_df=sdc_df)
 
-    def get_ranges_df(self, bin_size: int = 3, alpha: float = .05, min_bin=None, max_bin=None):
-        min_bin = int(np.floor(self.ts1.min())) if min_bin is None else min_bin
-        max_bin = int(np.ceil(self.ts1.max())) if max_bin is None else max_bin
-        df = (self.sdc_df
+    def get_ranges_df(self, bin_size: int = 3, alpha: float = .05, min_bin=None, max_bin=None, threshold: float = .0,
+                      ts: int = 1):
+        min_bin = int(np.floor(self.__dict__[f'ts{ts}'].min())) if min_bin is None else min_bin
+        max_bin = int(np.ceil(self.__dict__[f'ts{ts}'].max())) if max_bin is None else max_bin
+        name = self.__dict__[f'ts{ts}'].name
+        df = (self
+              .sdc_df
               .dropna()
               .assign(date_range=lambda dd:
-                      dd.date_1.apply(lambda x: pd.date_range(x, x + pd.to_timedelta(self.fragment_size, unit='days'))))
+        dd[f'date_{ts}'].apply(lambda x: pd.date_range(x, x + pd.to_timedelta(self.fragment_size, unit='days'))))
               [['r', 'p_value', 'date_range']]
               .explode('date_range')
               .rename(columns={'date_range': 'date'})
-              .merge(self.ts1.reset_index().rename(columns={'date_1': 'date', 'ts1': 'value'}))
-              .assign(cat_value=lambda dd: pd.cut(dd.value, bins=list(range(min_bin, max_bin + bin_size, bin_size)),
-                                                  precision=0))
-              )
-
-        n_df = df.groupby('cat_value').size().rename('n').reset_index()
-        df = (df.assign(significant=lambda dd: dd.p_value < alpha)
+              .reset_index()
+              .rename(columns={'index': 'comparison_id'})
+              .merge(self.__dict__[f'ts{ts}'].reset_index().rename(columns={f'date_{ts}': 'date', name: 'value'}))
+              .assign(cat_value=lambda dd:
+        pd.cut(dd.value, bins=list(range(min_bin, max_bin + bin_size, bin_size)), precision=0))
+              .groupby(['comparison_id'])
+              .apply(lambda dd: dd.cat_value.value_counts(True))
+              .loc[lambda x: x > threshold]
+              .reset_index()
+              .drop(columns='cat_value')
+              .rename(columns={'level_1': 'cat_value'})
+              .merge(self.sdc_df
+                     .reset_index()
+                     .rename(columns={'index': 'comparison_id'})
+                     [['r', 'p_value', 'comparison_id']])
+              .assign(significant=lambda dd: dd.p_value < alpha)
               .assign(direction=lambda dd: (dd.significant.astype(int) * ((dd.r > 0).astype(int) + 1))
                       .replace({0: 'NS', 1: 'Negative', 2: 'Positive'}))
               .assign(direction=lambda dd: pd.Categorical(dd.direction, categories=['Positive', 'Negative', 'NS'],
                                                           ordered=True))
               .groupby('cat_value')
-              .apply(lambda dd: dd.direction.value_counts().rename('counts').reset_index())
+              .apply(lambda dd: dd['direction'].value_counts().rename('counts').reset_index())
               .reset_index()
               .drop(columns='level_1')
               .rename(columns={'index': 'direction'})
-              .merge(n_df)
-              .groupby('cat_value')
-              .apply(lambda dd: dd.assign(freq=(dd.counts / dd.n).fillna(0)))
-              .assign(label=lambda dd: (dd.freq * 100).round(1).astype(str) + ' %')
+              .pipe(lambda dd:
+                    dd.merge(dd.groupby('cat_value', as_index=False)['counts'].sum().rename(columns={'counts': 'n'}),
+                             on='cat_value'))
+              .assign(freq=lambda dd: (dd['counts'] / dd['n']).fillna(0))
+              .assign(label=lambda dd: (dd['freq'] * 100).round(1).astype(str) + ' %')
               )
+
         return df
 
-    def plot_range_comparison(self, xlabel: str = '', figsize: Tuple[int] = (7, 3), **kwargs):
+    def plot_range_comparison(self, xlabel: str = '', figsize: Tuple[int] = (7, 3), add_text_label: bool = True,
+                              **kwargs):
         df = self.get_ranges_df(**kwargs)
         fig = (p9.ggplot(df)
                + p9.aes('cat_value', 'counts', fill='direction')
                + p9.geom_col(alpha=.8)
-               + p9.theme(figure_size=figsize)
+               + p9.theme(figure_size=figsize, axis_text_x=p9.element_text(rotation=45))
                + p9.scale_fill_manual(['#3f7f93', '#da3b46', '#4d4a4a'])
                + p9.labs(x=xlabel, y='Number of Comparisons', fill='R')
                )
 
-        if df.loc[df.direction == 'Positive'].loc[df.counts > 0].size > 0:
-            fig += p9.geom_text(p9.aes(label='label', x='cat_value', y='n + max(n) * .15'), inherit_aes=False, size=9,
-                                data=df.loc[df.direction == 'Positive'].loc[df.counts > 0], color='#3f7f93')
-        if df.loc[df.direction == 'Negative'].loc[df.counts > 0].size > 0:
-            fig += p9.geom_text(p9.aes(label='label', x='cat_value', y='n + max(n) * .05'), inherit_aes=False, size=9,
-                                data=df.loc[df.direction == 'Negative'].loc[df.counts > 0], color='#da3b46')
-        return fig.draw()
+        if add_text_label:
+            if df.loc[df.direction == 'Positive'].loc[df.counts > 0].size > 0:
+                fig += p9.geom_text(p9.aes(label='label', x='cat_value', y='n + max(n) * .15'),
+                                    inherit_aes=False, size=9,
+                                    data=df.loc[df.direction == 'Positive'].loc[df.counts > 0], color='#3f7f93')
+            if df.loc[df.direction == 'Negative'].loc[df.counts > 0].size > 0:
+                fig += p9.geom_text(p9.aes(label='label', x='cat_value', y='n + max(n) * .05'),
+                                    inherit_aes=False, size=9,
+                                    data=df.loc[df.direction == 'Negative'].loc[df.counts > 0], color='#da3b46')
+
+        return fig
 
     def plot_consecutive(self, alpha: float = .05, **kwargs):
         f = (self.sdc_df
              .loc[lambda dd: dd.p_value < alpha]
              # Here I make groups of consecutive significant values and report the longest for each lag.
              .groupby('lag', as_index=True)
              .apply(lambda gdf: gdf
```

### Comparing `sdcpy-0.2.0/sdcpy.egg-info/PKG-INFO` & `sdcpy-0.2.2/sdcpy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 1.1
 Name: sdcpy
-Version: 0.2.0
-Summary: Linear and non-linear Time Series Analysis methods.
+Version: 0.2.2
+Summary: Scale dependent correlation in Python.
 Home-page: https://github.com/AlFontal/sdcpy
 Author: Alejandro Fontal
 Author-email: alejandrofontal92@gmail.com
 License: MIT license
 Description: ======
         sdcpy
         ======
@@ -20,15 +20,15 @@
         .. image:: https://readthedocs.org/projects/sdcpy/badge/?version=latest
                 :target: https://sdcpy.readthedocs.io/en/latest/?badge=latest
                 :alt: Documentation Status
         
         
         
         
-        Scale Dependent Correlation (SDC) analysis [1, 2] in Python.
+        Scale Dependent Correlation (SDC) analysis [1, 2, 3] in Python.
         
         
         * Free software: MIT license
         * Documentation: https://sdcpy.readthedocs.io.
         
         
         Features
@@ -47,17 +47,19 @@
         ::
         
            pip install sdcpy
         
         References
         -----------
         
-        1. Rodríguez-Arias, Miquel Àngel, and Xavier Rodó. "A primer on the study of transitory dynamics in ecological series using the scale-dependent correlation analysis." Oecologia 138, no. 4 (2004): 485-504.
+        1. Rodó, X. (2001). Reversal of three global atmospheric fields linking changes in SST anomalies in the Pacific, Atlantic and Indian oceans at tropical latitudes and midlatitudes. ***Climate Dynamics***, 18:203-217. DOI: 10.1007/s003820100171.
         
-        2. Rodó, Xavier, and Miquel-Àngel Rodríguez-Arias. "A new method to detect transitory signatures and local time/space variability structures in the climate system: the scale-dependent correlation analysis." Climate Dynamics 27, no. 5 (2006): 441-458.
+        2. Rodríguez, M.A. & Rodó, X. (2004). A primer on the study of transitory dynamics in ecological series using the scale-dependent correlation analysis. ***Oecologia***, 138,485-504. DOI: 10.1007/s00442-003-1464-4.
+        
+        3. Rodó, X. & M.A. Rodriguez-Arias. (2006). A new method to detect transitory signatures and local time/space variability structures in the climate system: the scale-dependent correlation analysis. ***Climate Dynamics***, 27:441-458. DOI: 10.1007/s00382-005-0106-4.
         
         
         =======
         History
         =======
         
         0.1.0 (2020-10-09)
```

### Comparing `sdcpy-0.2.0/sdcpy.egg-info/SOURCES.txt` & `sdcpy-0.2.2/sdcpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sdcpy-0.2.0/setup.cfg` & `sdcpy-0.2.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.2.0
+current_version = 0.2.2
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
```

### Comparing `sdcpy-0.2.0/setup.py` & `sdcpy-0.2.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,22 +23,22 @@
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3.8',
     ],
-    description="Linear and non-linear Time Series Analysis methods.",
+    description="Scale dependent correlation in Python.",
     install_requires=requirements,
     license="MIT license",
     long_description=readme + '\n\n' + history,
     include_package_data=True,
     keywords='sdcpy',
     name='sdcpy',
     packages=find_packages(include=['sdcpy']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/AlFontal/sdcpy',
-    version='0.2.0',
+    version='0.2.2',
     zip_safe=False,
 )
```

### Comparing `sdcpy-0.2.0/tests/test_sdcpy.py` & `sdcpy-0.2.2/tests/test_sdcpy.py`

 * *Files identical despite different names*

