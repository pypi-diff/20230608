# Comparing `tmp/sdcpy-0.2.2.tar.gz` & `tmp/sdcpy-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdcpy-0.2.2.tar", last modified: Mon Feb 15 13:47:43 2021, max compression
+gzip compressed data, was "sdcpy-0.2.3.tar", max compression
```

## Comparing `sdcpy-0.2.2.tar` & `sdcpy-0.2.3.tar`

### file list

```diff
@@ -1,34 +1,6 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-15 13:47:43.016921 sdcpy-0.2.2/
--rw-rw-r--   0 travis    (2000) travis    (2000)      169 2021-02-15 13:44:57.000000 sdcpy-0.2.2/AUTHORS.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     3485 2021-02-15 13:44:57.000000 sdcpy-0.2.2/CONTRIBUTING.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       89 2021-02-15 13:44:57.000000 sdcpy-0.2.2/HISTORY.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1075 2021-02-15 13:44:57.000000 sdcpy-0.2.2/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      262 2021-02-15 13:44:57.000000 sdcpy-0.2.2/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     2681 2021-02-15 13:47:43.016921 sdcpy-0.2.2/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1599 2021-02-15 13:44:57.000000 sdcpy-0.2.2/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-15 13:47:43.016921 sdcpy-0.2.2/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)      606 2021-02-15 13:44:57.000000 sdcpy-0.2.2/docs/Makefile
--rw-rw-r--   0 travis    (2000) travis    (2000)       28 2021-02-15 13:44:57.000000 sdcpy-0.2.2/docs/authors.rst
--rwxrwxr-x   0 travis    (2000) travis    (2000)     4795 2021-02-15 13:44:57.000000 sdcpy-0.2.2/docs/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       33 2021-02-15 13:44:57.000000 sdcpy-0.2.2/docs/contributing.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       28 2021-02-15 13:44:57.000000 sdcpy-0.2.2/docs/history.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      302 2021-02-15 13:44:57.000000 sdcpy-0.2.2/docs/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1098 2021-02-15 13:44:57.000000 sdcpy-0.2.2/docs/installation.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      803 2021-02-15 13:44:57.000000 sdcpy-0.2.2/docs/make.bat
--rw-rw-r--   0 travis    (2000) travis    (2000)       27 2021-02-15 13:44:57.000000 sdcpy-0.2.2/docs/readme.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       65 2021-02-15 13:44:57.000000 sdcpy-0.2.2/docs/usage.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      100 2021-02-15 13:46:10.000000 sdcpy-0.2.2/pyproject.toml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-15 13:47:43.016921 sdcpy-0.2.2/sdcpy/
--rw-rw-r--   0 travis    (2000) travis    (2000)      161 2021-02-15 13:44:57.000000 sdcpy-0.2.2/sdcpy/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    26998 2021-02-15 13:44:57.000000 sdcpy-0.2.2/sdcpy/scale_dependent_correlation.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-15 13:47:43.016921 sdcpy-0.2.2/sdcpy.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2681 2021-02-15 13:47:42.000000 sdcpy-0.2.2/sdcpy.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      517 2021-02-15 13:47:42.000000 sdcpy-0.2.2/sdcpy.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-02-15 13:47:42.000000 sdcpy-0.2.2/sdcpy.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-02-15 13:44:59.000000 sdcpy-0.2.2/sdcpy.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)       52 2021-02-15 13:47:42.000000 sdcpy-0.2.2/sdcpy.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        6 2021-02-15 13:47:42.000000 sdcpy-0.2.2/sdcpy.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      561 2021-02-15 13:47:43.016921 sdcpy-0.2.2/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1246 2021-02-15 13:44:57.000000 sdcpy-0.2.2/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-15 13:47:43.016921 sdcpy-0.2.2/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)      605 2021-02-15 13:44:57.000000 sdcpy-0.2.2/tests/test_sdcpy.py
+-rw-r--r--   0        0        0     1075 2022-10-03 08:37:30.165063 sdcpy-0.2.3/LICENSE
+-rw-r--r--   0        0        0        7 2023-06-08 08:32:43.194160 sdcpy-0.2.3/README.md
+-rw-r--r--   0        0        0      580 2023-06-08 08:08:39.040837 sdcpy-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      161 2022-10-03 08:37:30.165892 sdcpy-0.2.3/sdcpy/__init__.py
+-rwxr-xr-x   0        0        0    27142 2023-06-07 15:35:29.289477 sdcpy-0.2.3/sdcpy/scale_dependent_correlation.py
+-rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 sdcpy-0.2.3/PKG-INFO
```

### Comparing `sdcpy-0.2.2/LICENSE` & `sdcpy-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sdcpy-0.2.2/sdcpy/scale_dependent_correlation.py` & `sdcpy-0.2.3/sdcpy/scale_dependent_correlation.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,24 +9,23 @@
 
 from matplotlib import ticker
 from scipy import stats
 from scipy.stats.mstats import rankdata
 from tqdm.auto import tqdm
 from typing import Callable, Union, Optional, Tuple
 
-plt.style.use('seaborn-white')
+plt.style.use('seaborn-v0_8-white')
 
 RECOGNIZED_METHODS = {
     'pearson': lambda x, y: stats.pearsonr(x, y),
     'spearman': lambda x, y: stats.spearmanr(x, y),
-    'kendall': lambda x, y: stats.kendalltau(x, y),
 }
 
-CONSTANT_WARNING = {'pearson': stats.PearsonRConstantInputWarning,
-                    'spearman': stats.SpearmanRConstantInputWarning}
+CONSTANT_WARNING = {'pearson': stats.ConstantInputWarning,
+                    'spearman': stats.ConstantInputWarning}
 
 
 def generate_correlation_map(x: np.ndarray, y: np.ndarray, method: str = 'pearson') -> np.ndarray:
     """
     Correlate each row in matrix X against each row in matrix Y.
 
     Parameters
@@ -190,36 +189,44 @@
     p9.ggplot.ggplot
         Plot
     """
     fragment_size = int(sdc_df.iloc[0]['stop_1'] - sdc_df.iloc[0]['start_1'])
     f = (sdc_df
          .loc[lambda dd: dd.p_value < alpha]
          .assign(r_str=lambda dd: dd['r'].apply(lambda x: '$r > 0$' if x > 0 else '$r < 0$'))
-         .pipe(lambda dd: p9.ggplot(dd)
-                          + p9.aes('start_1', 'start_2', fill='r_str', alpha='abs(r)')
-                          + p9.geom_tile()
-                          + p9.scale_fill_manual(['#da2421', 'black'])
-                          + p9.scale_y_reverse()
-                          + p9.theme(**kwargs)
-                          + p9.guides(alpha=False)
-                          + p9.labs(x='$X_i$', y='$Y_j$', fill='$r$',
-                                    title=f'Two-Way SDC plot for $S = {fragment_size}$' + r' and $\alpha =$' +
-                                          f'{alpha}')
+         .pipe(lambda dd: 
+         p9.ggplot(dd)
+       + p9.aes('start_1', 'start_2', fill='r_str', alpha='abs(r)')
+       + p9.geom_tile()
+       + p9.scale_fill_manual(['#da2421', 'black'])
+       + p9.scale_y_reverse()
+       + p9.theme(**kwargs)
+       + p9.guides(alpha=False)
+       + p9.labs(x='$X_i$', y='$Y_j$', fill='$r$',
+                 title=f'Two-Way SDC plot for $S = {fragment_size}$' + r' and $\alpha =$' +
+                       f'{alpha}')
                )
          )
 
     return f
 
 
 class SDCAnalysis:
     def __init__(self, ts1: np.ndarray, ts2: np.ndarray = None, fragment_size: int = 7, n_permutations: int = 99,
                  method: Union[str, Callable] = 'pearson', two_tailed: bool = True, permutations: bool = True,
                  sdc_df: Optional[pd.DataFrame] = None, min_lag: int = -np.inf, max_lag: int = np.inf):
         self.way = 'one-way' if ts2 is None else 'two-way'  # One-way SDC inferred if no ts2 is provided
         ts2 = ts1.copy() if self.way == 'one-way' else ts2
+        # TODO: As mentioned in (#4), we should make 
+        if not isinstance(ts1, pd.Series):
+            ts1 = pd.Series(ts1, 
+            index=pd.date_range(start='2000-01-01', periods=len(ts1), freq='D'))
+        if not isinstance(ts2, pd.Series):
+            ts2 = pd.Series(ts2, 
+            index=pd.date_range(start='2000-01-01', periods=len(ts2), freq='D'))
         min_date = max(ts1.index.min(), ts2.index.min())
         max_date = min(ts1.index.max(), ts2.index.max())
         self.ts1 = ts1[min_date:max_date]
         self.ts2 = ts2[min_date:max_date]
         self.fragment_size = fragment_size
         self.n_permutations = n_permutations
         self.ts1.index.name = 'date_1'
@@ -404,16 +411,16 @@
         ts2 = fig.add_subplot(gs[2:4, 0])
         plt.plot(self.ts2, self.ts2.reset_index()['date_2'], color='black')
         # Heat map
         hm = fig.add_subplot(gs[2:4, 1:3])
 
         (self.sdc_df
          .loc[lambda dd: (dd.lag <= max_lag) & (dd.lag >= min_lag)]
-         .pipe(lambda dd: sns.heatmap(dd.pivot('date_2', 'date_1', 'r'), cbar=False,
-                                      mask=dd.pivot('date_2', 'date_1', 'p_value') > alpha,
+         .pipe(lambda dd: sns.heatmap(dd.pivot(index='date_2', columns='date_1', values='r'), cbar=False,
+                                      mask=dd.pivot(index='date_2', columns='date_1', values='p_value') > alpha,
                                       cmap=sns.diverging_palette(10, 220, sep=80, n=20), ax=hm))
          )
         # Add identity line to ease shift visualization
         identity_len = min(len(self.ts1), len(self.ts2)) - self.fragment_size + 1
         plt.plot(range(identity_len), range(identity_len), linestyle=':', color='black', alpha=.8)
         # Correct and format ticks, labels, grids
         # Hide Heatmap labels and ticks
@@ -462,15 +469,14 @@
         # Max Correlations
         colors = {'Max $r$': '#3f7f93', 'Min $r$ (abs)': '#da3b46'}
         if min_lag < 0:
             mc1 = fig.add_subplot(gs[-1, 1:3])
             (self.sdc_df
              .loc[lambda dd: dd.p_value < alpha]
              .loc[lambda dd: (dd.lag <= max_lag) & (dd.lag >= min_lag)]
-             #.loc[lambda dd: dd['r'] < 0]
              .groupby('date_1')
              .apply(lambda dd: dd.loc[dd['r'].abs() == dd['r'].abs().max()].loc[lambda d: d['lag'] == d['lag'].min()])
              .reset_index(drop=True)
              .groupby('date_1')
              .agg(r_max=('r', lambda x: x.where(x > 0).max()), r_min=('r', lambda x: abs(x.where(x < 0).min())))
              .rename(columns={'r_max': 'Max $r$', 'r_min': 'Min $r$ (abs)'})
              .reset_index()
```

