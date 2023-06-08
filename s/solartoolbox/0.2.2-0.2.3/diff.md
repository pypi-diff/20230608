# Comparing `tmp/solartoolbox-0.2.2.tar.gz` & `tmp/solartoolbox-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solartoolbox-0.2.2.tar", last modified: Wed Jul 27 19:10:26 2022, max compression
+gzip compressed data, was "solartoolbox-0.2.3.tar", last modified: Thu Jun  8 17:51:50 2023, max compression
```

## Comparing `solartoolbox-0.2.2.tar` & `solartoolbox-0.2.3.tar`

### file list

```diff
@@ -1,30 +1,34 @@
-drwxrwxrwx   0        0        0        0 2022-07-27 19:10:26.023245 solartoolbox-0.2.2/
--rw-rw-rw-   0        0        0     1548 2021-07-12 14:12:05.000000 solartoolbox-0.2.2/LICENSE
--rw-rw-rw-   0        0        0     5753 2022-07-27 19:10:26.023245 solartoolbox-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     5324 2022-07-27 18:46:13.000000 solartoolbox-0.2.2/README.md
--rw-rw-rw-   0        0        0       86 2022-05-27 13:41:43.000000 solartoolbox-0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       86 2022-07-27 19:10:26.027234 solartoolbox-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      969 2022-07-27 18:46:13.000000 solartoolbox-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2022-07-27 19:10:25.936606 solartoolbox-0.2.2/src/
-drwxrwxrwx   0        0        0        0 2022-07-27 19:10:25.967726 solartoolbox-0.2.2/src/solartoolbox/
--rw-rw-rw-   0        0        0       41 2022-07-27 18:42:41.000000 solartoolbox-0.2.2/src/solartoolbox/__init__.py
--rw-rw-rw-   0        0        0    15956 2022-05-27 14:01:17.000000 solartoolbox-0.2.2/src/solartoolbox/cmv.py
-drwxrwxrwx   0        0        0        0 2022-07-27 19:10:26.009475 solartoolbox-0.2.2/src/solartoolbox/dataio/
--rw-rw-rw-   0        0        0        0 2021-07-12 14:12:05.000000 solartoolbox-0.2.2/src/solartoolbox/dataio/__init__.py
--rw-rw-rw-   0        0        0    12690 2022-06-15 13:44:48.000000 solartoolbox-0.2.2/src/solartoolbox/dataio/hope_campaign.py
--rw-rw-rw-   0        0        0     2593 2022-06-15 13:43:26.000000 solartoolbox-0.2.2/src/solartoolbox/dataio/iotools.py
--rw-rw-rw-   0        0        0     6153 2022-06-15 13:55:33.000000 solartoolbox-0.2.2/src/solartoolbox/dataio/nrcan_data.py
--rw-rw-rw-   0        0        0     2764 2022-05-25 16:29:49.000000 solartoolbox-0.2.2/src/solartoolbox/dataio/surfrad.py
--rw-rw-rw-   0        0        0    14647 2022-07-27 19:04:27.000000 solartoolbox-0.2.2/src/solartoolbox/signalproc.py
--rw-rw-rw-   0        0        0     1251 2022-07-27 18:42:41.000000 solartoolbox-0.2.2/src/solartoolbox/solartoolbox.py
--rw-rw-rw-   0        0        0    12100 2021-10-25 17:11:55.000000 solartoolbox-0.2.2/src/solartoolbox/spatial.py
--rw-rw-rw-   0        0        0    16176 2022-05-25 14:14:13.000000 solartoolbox-0.2.2/src/solartoolbox/stats.py
-drwxrwxrwx   0        0        0        0 2022-07-27 19:10:26.022216 solartoolbox-0.2.2/src/solartoolbox/visualization/
--rw-rw-rw-   0        0        0       24 2021-10-25 17:11:55.000000 solartoolbox-0.2.2/src/solartoolbox/visualization/__init__.py
--rw-rw-rw-   0        0        0     1827 2021-10-25 17:11:55.000000 solartoolbox-0.2.2/src/solartoolbox/visualization/vis_tools.py
-drwxrwxrwx   0        0        0        0 2022-07-27 19:10:25.983685 solartoolbox-0.2.2/src/solartoolbox.egg-info/
--rw-rw-rw-   0        0        0     5753 2022-07-27 19:10:25.000000 solartoolbox-0.2.2/src/solartoolbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      693 2022-07-27 19:10:25.000000 solartoolbox-0.2.2/src/solartoolbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-27 19:10:25.000000 solartoolbox-0.2.2/src/solartoolbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       83 2022-07-27 19:10:25.000000 solartoolbox-0.2.2/src/solartoolbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-07-27 19:10:25.000000 solartoolbox-0.2.2/src/solartoolbox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-08 17:51:50.793497 solartoolbox-0.2.3/
+-rw-rw-rw-   0        0        0     1548 2021-07-12 14:12:05.000000 solartoolbox-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0     5841 2023-06-08 17:51:50.793497 solartoolbox-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5412 2023-06-08 17:50:46.000000 solartoolbox-0.2.3/README.md
+-rw-rw-rw-   0        0        0       86 2022-05-27 13:41:43.000000 solartoolbox-0.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-06-08 17:51:50.794447 solartoolbox-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      969 2023-06-08 17:47:53.000000 solartoolbox-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 17:51:50.646662 solartoolbox-0.2.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-08 17:51:50.703098 solartoolbox-0.2.3/src/solartoolbox/
+-rw-rw-rw-   0        0        0       41 2022-07-27 18:42:41.000000 solartoolbox-0.2.3/src/solartoolbox/__init__.py
+-rw-rw-rw-   0        0        0    15956 2022-05-27 14:01:17.000000 solartoolbox-0.2.3/src/solartoolbox/cmv.py
+drwxrwxrwx   0        0        0        0 2023-06-08 17:51:50.754960 solartoolbox-0.2.3/src/solartoolbox/dataio/
+-rw-rw-rw-   0        0        0        0 2021-07-12 14:12:05.000000 solartoolbox-0.2.3/src/solartoolbox/dataio/__init__.py
+-rw-rw-rw-   0        0        0    12690 2022-06-15 13:44:48.000000 solartoolbox-0.2.3/src/solartoolbox/dataio/hope_campaign.py
+-rw-rw-rw-   0        0        0     2593 2022-06-15 13:43:26.000000 solartoolbox-0.2.3/src/solartoolbox/dataio/iotools.py
+-rw-rw-rw-   0        0        0     6153 2022-06-15 13:55:33.000000 solartoolbox-0.2.3/src/solartoolbox/dataio/nrcan_data.py
+-rw-rw-rw-   0        0        0     2764 2022-05-25 16:29:49.000000 solartoolbox-0.2.3/src/solartoolbox/dataio/surfrad.py
+-rw-rw-rw-   0        0        0    20185 2023-06-08 17:47:53.000000 solartoolbox-0.2.3/src/solartoolbox/signalproc.py
+-rw-rw-rw-   0        0        0     1251 2022-07-27 18:42:41.000000 solartoolbox-0.2.3/src/solartoolbox/solartoolbox.py
+-rw-rw-rw-   0        0        0    12100 2021-10-25 17:11:55.000000 solartoolbox-0.2.3/src/solartoolbox/spatial.py
+-rw-rw-rw-   0        0        0    16176 2022-05-25 14:14:13.000000 solartoolbox-0.2.3/src/solartoolbox/stats.py
+drwxrwxrwx   0        0        0        0 2023-06-08 17:51:50.770509 solartoolbox-0.2.3/src/solartoolbox/visualization/
+-rw-rw-rw-   0        0        0       24 2021-10-25 17:11:55.000000 solartoolbox-0.2.3/src/solartoolbox/visualization/__init__.py
+-rw-rw-rw-   0        0        0     1827 2021-10-25 17:11:55.000000 solartoolbox-0.2.3/src/solartoolbox/visualization/vis_tools.py
+drwxrwxrwx   0        0        0        0 2023-06-08 17:51:50.722048 solartoolbox-0.2.3/src/solartoolbox.egg-info/
+-rw-rw-rw-   0        0        0     5841 2023-06-08 17:51:50.000000 solartoolbox-0.2.3/src/solartoolbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      762 2023-06-08 17:51:50.000000 solartoolbox-0.2.3/src/solartoolbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 17:51:50.000000 solartoolbox-0.2.3/src/solartoolbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2023-06-08 17:51:50.000000 solartoolbox-0.2.3/src/solartoolbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-08 17:51:50.000000 solartoolbox-0.2.3/src/solartoolbox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-08 17:51:50.791489 solartoolbox-0.2.3/tests/
+-rw-rw-rw-   0        0        0     2463 2022-07-27 18:42:41.000000 solartoolbox-0.2.3/tests/test_solartoolbox.py
+-rw-rw-rw-   0        0        0    13287 2021-10-25 17:11:55.000000 solartoolbox-0.2.3/tests/test_spatial.py
+-rw-rw-rw-   0        0        0     8888 2022-05-25 15:03:49.000000 solartoolbox-0.2.3/tests/test_stats.py
```

### Comparing `solartoolbox-0.2.2/LICENSE` & `solartoolbox-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `solartoolbox-0.2.2/PKG-INFO` & `solartoolbox-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: solartoolbox
-Version: 0.2.2
+Version: 0.2.3
 Summary: A research toolbox for solar analysis
 Home-page: https://github.com/jranalli/solartoolbox
-Download-URL: https://github.com/jranalli/solartoolbox/archive/0.2.2.tar.gz
+Download-URL: https://github.com/jranalli/solartoolbox/archive/0.2.3.tar.gz
 Author: Joe Ranalli
 Author-email: jranalli@psu.edu
 License: BSD (3 Clause)
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: demos
 License-File: LICENSE
@@ -118,14 +118,16 @@
 ##### Version 0.2
 First public release
 ##### Version 0.2.1
 Add wrapper for `pvlib.clearsky_index` to handle pandas type
 ##### Version 0.2.2
 Change input to camfilter to handle references that don't coincide with the 
 site itself. This change breaks code!
+##### Version 0.2.3
+Add methods for calculating delay between signals to `signalproc`
 
 ## Author
 Joe Ranalli  
 Associate Professor of Engineering  
 Penn State Hazleton  
 jar339@psu.edu  
 http://personal.psu.edu/jar339/
```

### Comparing `solartoolbox-0.2.2/README.md` & `solartoolbox-0.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,16 @@
 ##### Version 0.2
 First public release
 ##### Version 0.2.1
 Add wrapper for `pvlib.clearsky_index` to handle pandas type
 ##### Version 0.2.2
 Change input to camfilter to handle references that don't coincide with the 
 site itself. This change breaks code!
+##### Version 0.2.3
+Add methods for calculating delay between signals to `signalproc`
 
 ## Author
 Joe Ranalli  
 Associate Professor of Engineering  
 Penn State Hazleton  
 jar339@psu.edu  
 http://personal.psu.edu/jar339/
```

### Comparing `solartoolbox-0.2.2/setup.py` & `solartoolbox-0.2.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-ver = '0.2.2'
+ver = '0.2.3'
 
 
 setup(
     name='solartoolbox',
     version=ver,
     author="Joe Ranalli",
     author_email="jranalli@psu.edu",
```

### Comparing `solartoolbox-0.2.2/src/solartoolbox/cmv.py` & `solartoolbox-0.2.3/src/solartoolbox/cmv.py`

 * *Files identical despite different names*

### Comparing `solartoolbox-0.2.2/src/solartoolbox/dataio/hope_campaign.py` & `solartoolbox-0.2.3/src/solartoolbox/dataio/hope_campaign.py`

 * *Files identical despite different names*

### Comparing `solartoolbox-0.2.2/src/solartoolbox/dataio/iotools.py` & `solartoolbox-0.2.3/src/solartoolbox/dataio/iotools.py`

 * *Files identical despite different names*

### Comparing `solartoolbox-0.2.2/src/solartoolbox/dataio/nrcan_data.py` & `solartoolbox-0.2.3/src/solartoolbox/dataio/nrcan_data.py`

 * *Files identical despite different names*

### Comparing `solartoolbox-0.2.2/src/solartoolbox/dataio/surfrad.py` & `solartoolbox-0.2.3/src/solartoolbox/dataio/surfrad.py`

 * *Files identical despite different names*

### Comparing `solartoolbox-0.2.2/src/solartoolbox/signalproc.py` & `solartoolbox-0.2.3/src/solartoolbox/signalproc.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import numpy as np
 import pandas as pd
 from scipy import signal
 from scipy.interpolate import interp1d
+from scipy.optimize import curve_fit
 import pvlib
 
-from solartoolbox import spatial
+from solartoolbox import spatial, stats
 
 
 # Library for Analyzing Time Series Transfer Functions
 def averaged_psd(input_tsig, navgs, overlap=0.5,
                  window='hanning', detrend='linear', scaling='density'):
     """
     Calculate an averaged power spectral density for a signal.
@@ -165,14 +166,165 @@
         interp_filt = pd.Series(interp_filt[:, 0], index=new_freq)
     else:
         interp_filt = pd.DataFrame(interp_filt, columns=input_tf.columns,
                                    index=new_freq)
     return interp_filt
 
 
+def tf_delay(tf, coh_limit=0.6, freq_limit=0.02, method='fit'):
+    """
+    Compute the delay based on the phase of a transfer function
+
+    Parameters
+    ----------
+    tf : pd.DataFrame
+        The transfer function, produced by signalproc.averaged_tf. Critically,
+        it needs to have columns of 'tf' and 'coh' in order to use the limit.
+    coh_limit : float
+        The coherence limit to use for filtering the phase. Set to None to
+        include all points.
+    freq_limit : float
+        The frequency limit to use for filtering the phase. Set to None to
+        include all points.
+    method : str
+        The method to use for computing the delay. Options are:
+            'diff' - unwrap phase and take derivative
+            'fit' - fit a line to the phase
+
+    Returns
+    -------
+    delay : float
+        The delay in seconds
+
+    """
+    try:
+        if coh_limit is None:
+            ix1 = np.ones_like(tf.index, dtype=bool)
+        else:
+            ix1 = tf['coh'] > coh_limit
+        if freq_limit is None:
+            ix2 = np.ones_like(tf.index, dtype=bool)
+        else:
+            ix2 = tf.index < freq_limit
+        ix = np.bitwise_and(ix1, ix2)
+    except KeyError:
+        from warnings import warn
+        warn('No coherence column found, using all points.')
+        ix = np.ones_like(tf.index, dtype=bool)
+
+    if method == 'diff':
+        # # Method 1: unwrap phase and take derivative
+        gd = -np.diff(np.unwrap(np.angle(tf)))/np.diff(tf.index)
+        gd = np.append(gd, gd[-1])
+        gd = gd/(2*np.pi)
+        avg_del = np.sum(gd * ix / np.sum(ix))
+        return avg_del, ix
+
+    # Method 2: curve fit the phase
+    elif method == 'fit':
+        def delay_fitter(x, delval):
+            """
+            Curve fit helper function for computing the group delay.
+            :param x: the transfer function frequency
+            :param delval: The 'real' phase to fit the group delay to
+            :return: the modeled phase
+            """
+            model = np.unwrap(np.angle(np.ones_like(x) *
+                                       np.exp(2 * np.pi * 1j * x * -delval)))
+            return model
+
+        try:
+            return curve_fit(delay_fitter, tf.index[ix],
+                             np.unwrap(np.angle(tf['tf'][ix])))[0], ix
+        except ValueError:
+            from warnings import warn
+            if not ix.any():
+                warn('Curve fit failed due to coherence limit. Returning NaN')
+                return np.nan, ix
+
+            else:
+                warn('Curve fit failed for unknown reason. Returning NaN')
+                return np.nan, ix
+
+    else:
+        raise ValueError(f'Invalid method: {method}')
+
+
+def xcorr_delay(ts_in, ts_out, scaling='coeff'):
+    """
+    Compute the delay between two timeseries using cross correlation.
+
+    Parameters
+    ----------
+    ts_in : pd.Series
+        The input timeseries. Requires that the index operate as datetime.
+    ts_out : pd.Series
+        The output timeseries
+    scaling : str
+        Type of scaling to use for cross correlation. Options are:
+
+        'energy' - scales by the energy of the autocorrelation of the input
+        'coeff' - scales the output to the correlation coefficient (always
+                  removes the mean from both signals)
+        'unbiased_energy' - similar to energy, but normalizes based on lag to
+                            account for the fewer points used in the
+                            convolution. Removes bias towards small lags.
+        'unbiased_coeff' - similar to coeff, but normalizes based on lag to
+                            account for the fewer points used in the
+                            convolution. Removes bias towards small lags.
+
+    Returns
+    -------
+    delay : float
+        Time lag between the two timeseries at the maximum value of the cross
+        correlation. Values are always integer multiples of the sampling period
+        as the max correlation values are limited to the discrete time steps.
+    corr : float
+        The peak value of the cross correlation at the identified delay.
+    """
+    # Method 3: Cross Correlation
+    xcorr_i, lags = stats.correlation(ts_in, ts_out, scaling)
+    dt = (ts_in.index[1] - ts_in.index[0]).total_seconds()
+    lags = lags * dt
+    peak_lag_index = xcorr_i.argmax()  # Index of peak correlation
+    delay = -lags[peak_lag_index]
+    return delay, xcorr_i[peak_lag_index]
+
+
+def apply_delay(tf, delay):
+    """
+    Apply a time delay to a transfer function. This is equivalent to rotating
+    the phase as a linear function of frequency.
+
+    To compare with a unity transfer function, consider:
+        apply_delay(tf['tf'] * 0 + 1, delay)
+
+    Parameters
+    ----------
+    tf : pd.DataFrame
+        The transfer function, produced by signalproc.averaged_tf. Critically,
+        it needs to have a column of 'tf' containing the complex valued
+        transfer function, and the index must contain the frequency in Hz.
+    delay : float
+        The delay to apply to the transfer function. Units are in seconds.
+
+    Returns
+    -------
+    A copy of the transfer function with the delay applied in rotating
+    the phase.
+    """
+
+    tf = tf.copy()
+
+    # Equation for rotating the phase by a delay
+    tf['tf'] = tf['tf'] * np.exp(2 * np.pi * 1j * tf.index * -delay)
+
+    return tf
+
+
 def get_1d_plant(centers, ref_center=0,
                  width=None, shape="square",
                  dx=1, xmax=500000):
     """
     Generate a one dimensional plant array based on a list of center positions.
     Plant is essentially a comb filter with a site of a given shape placed at
     each specified center position
```

### Comparing `solartoolbox-0.2.2/src/solartoolbox/solartoolbox.py` & `solartoolbox-0.2.3/src/solartoolbox/solartoolbox.py`

 * *Files identical despite different names*

### Comparing `solartoolbox-0.2.2/src/solartoolbox/spatial.py` & `solartoolbox-0.2.3/src/solartoolbox/spatial.py`

 * *Files identical despite different names*

### Comparing `solartoolbox-0.2.2/src/solartoolbox/stats.py` & `solartoolbox-0.2.3/src/solartoolbox/stats.py`

 * *Files identical despite different names*

### Comparing `solartoolbox-0.2.2/src/solartoolbox/visualization/vis_tools.py` & `solartoolbox-0.2.3/src/solartoolbox/visualization/vis_tools.py`

 * *Files identical despite different names*

### Comparing `solartoolbox-0.2.2/src/solartoolbox.egg-info/PKG-INFO` & `solartoolbox-0.2.3/src/solartoolbox.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: solartoolbox
-Version: 0.2.2
+Version: 0.2.3
 Summary: A research toolbox for solar analysis
 Home-page: https://github.com/jranalli/solartoolbox
-Download-URL: https://github.com/jranalli/solartoolbox/archive/0.2.2.tar.gz
+Download-URL: https://github.com/jranalli/solartoolbox/archive/0.2.3.tar.gz
 Author: Joe Ranalli
 Author-email: jranalli@psu.edu
 License: BSD (3 Clause)
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: demos
 License-File: LICENSE
@@ -118,14 +118,16 @@
 ##### Version 0.2
 First public release
 ##### Version 0.2.1
 Add wrapper for `pvlib.clearsky_index` to handle pandas type
 ##### Version 0.2.2
 Change input to camfilter to handle references that don't coincide with the 
 site itself. This change breaks code!
+##### Version 0.2.3
+Add methods for calculating delay between signals to `signalproc`
 
 ## Author
 Joe Ranalli  
 Associate Professor of Engineering  
 Penn State Hazleton  
 jar339@psu.edu  
 http://personal.psu.edu/jar339/
```

### Comparing `solartoolbox-0.2.2/src/solartoolbox.egg-info/SOURCES.txt` & `solartoolbox-0.2.3/src/solartoolbox.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -16,8 +16,11 @@
 src/solartoolbox.egg-info/top_level.txt
 src/solartoolbox/dataio/__init__.py
 src/solartoolbox/dataio/hope_campaign.py
 src/solartoolbox/dataio/iotools.py
 src/solartoolbox/dataio/nrcan_data.py
 src/solartoolbox/dataio/surfrad.py
 src/solartoolbox/visualization/__init__.py
-src/solartoolbox/visualization/vis_tools.py
+src/solartoolbox/visualization/vis_tools.py
+tests/test_solartoolbox.py
+tests/test_spatial.py
+tests/test_stats.py
```

