# Comparing `tmp/icecube-skyreader-1.1.0.tar.gz` & `tmp/icecube-skyreader-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icecube-skyreader-1.1.0.tar", last modified: Wed Jun  7 22:08:18 2023, max compression
+gzip compressed data, was "icecube-skyreader-1.2.0.tar", last modified: Wed Jun  7 23:40:14 2023, max compression
```

## Comparing `icecube-skyreader-1.1.0.tar` & `icecube-skyreader-1.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 22:08:18.950540 icecube-skyreader-1.1.0/
--rw-r--r--   0 root         (0) root         (0)     1085 2023-06-07 22:08:16.000000 icecube-skyreader-1.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1987 2023-06-07 22:08:18.950540 icecube-skyreader-1.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1025 2023-06-07 22:08:16.000000 icecube-skyreader-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 22:08:18.950540 icecube-skyreader-1.1.0/icecube_skyreader.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1987 2023-06-07 22:08:18.000000 icecube-skyreader-1.1.0/icecube_skyreader.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      389 2023-06-07 22:08:18.000000 icecube-skyreader-1.1.0/icecube_skyreader.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 22:08:18.000000 icecube-skyreader-1.1.0/icecube_skyreader.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      120 2023-06-07 22:08:18.000000 icecube-skyreader-1.1.0/icecube_skyreader.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-07 22:08:18.000000 icecube-skyreader-1.1.0/icecube_skyreader.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1762 2023-06-07 22:08:18.950540 icecube-skyreader-1.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       76 2023-06-07 22:08:16.000000 icecube-skyreader-1.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 22:08:18.950540 icecube-skyreader-1.1.0/skyreader/
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-07 22:08:16.000000 icecube-skyreader-1.1.0/skyreader/__init__.py
--rw-r--r--   0 root         (0) root         (0)      915 2023-06-07 22:08:16.000000 icecube-skyreader-1.1.0/skyreader/event_metadata.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 22:08:18.950540 icecube-skyreader-1.1.0/skyreader/plot/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 22:08:16.000000 icecube-skyreader-1.1.0/skyreader/plot/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9057 2023-06-07 22:08:16.000000 icecube-skyreader-1.1.0/skyreader/plot/plotting_tools.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 22:08:16.000000 icecube-skyreader-1.1.0/skyreader/py.typed
--rw-r--r--   0 root         (0) root         (0)    48327 2023-06-07 22:08:16.000000 icecube-skyreader-1.1.0/skyreader/result.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 23:40:14.567318 icecube-skyreader-1.2.0/
+-rw-r--r--   0 root         (0) root         (0)     1085 2023-06-07 23:40:12.000000 icecube-skyreader-1.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1987 2023-06-07 23:40:14.567318 icecube-skyreader-1.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1025 2023-06-07 23:40:12.000000 icecube-skyreader-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 23:40:14.567318 icecube-skyreader-1.2.0/icecube_skyreader.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1987 2023-06-07 23:40:14.000000 icecube-skyreader-1.2.0/icecube_skyreader.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      389 2023-06-07 23:40:14.000000 icecube-skyreader-1.2.0/icecube_skyreader.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 23:40:14.000000 icecube-skyreader-1.2.0/icecube_skyreader.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      120 2023-06-07 23:40:14.000000 icecube-skyreader-1.2.0/icecube_skyreader.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-07 23:40:14.000000 icecube-skyreader-1.2.0/icecube_skyreader.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1762 2023-06-07 23:40:14.571318 icecube-skyreader-1.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       76 2023-06-07 23:40:12.000000 icecube-skyreader-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 23:40:14.567318 icecube-skyreader-1.2.0/skyreader/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-07 23:40:12.000000 icecube-skyreader-1.2.0/skyreader/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      915 2023-06-07 23:40:12.000000 icecube-skyreader-1.2.0/skyreader/event_metadata.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 23:40:14.567318 icecube-skyreader-1.2.0/skyreader/plot/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 23:40:12.000000 icecube-skyreader-1.2.0/skyreader/plot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9057 2023-06-07 23:40:12.000000 icecube-skyreader-1.2.0/skyreader/plot/plotting_tools.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 23:40:12.000000 icecube-skyreader-1.2.0/skyreader/py.typed
+-rw-r--r--   0 root         (0) root         (0)    46823 2023-06-07 23:40:12.000000 icecube-skyreader-1.2.0/skyreader/result.py
```

### Comparing `icecube-skyreader-1.1.0/LICENSE` & `icecube-skyreader-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `icecube-skyreader-1.1.0/PKG-INFO` & `icecube-skyreader-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icecube-skyreader
-Version: 1.1.0
+Version: 1.2.0
 Summary: An API for Results Produced by SkyDriver & the Skymap Scanner
 Home-page: https://github.com/icecube/skyreader
 Download-URL: https://pypi.org/project/icecube-skyreader/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/icecube/skyreader/issues
```

### Comparing `icecube-skyreader-1.1.0/README.md` & `icecube-skyreader-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `icecube-skyreader-1.1.0/icecube_skyreader.egg-info/PKG-INFO` & `icecube-skyreader-1.2.0/icecube_skyreader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icecube-skyreader
-Version: 1.1.0
+Version: 1.2.0
 Summary: An API for Results Produced by SkyDriver & the Skymap Scanner
 Home-page: https://github.com/icecube/skyreader
 Download-URL: https://pypi.org/project/icecube-skyreader/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/icecube/skyreader/issues
```

### Comparing `icecube-skyreader-1.1.0/setup.cfg` & `icecube-skyreader-1.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `icecube-skyreader-1.1.0/skyreader/__init__.py` & `icecube-skyreader-1.2.0/skyreader/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,14 @@
 # version is a human-readable version number.
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
-__version__ = "1.1.0"
+__version__ = "1.2.0"
 version_info = (
     int(__version__.split(".")[0]),
     int(__version__.split(".")[1]),
     int(__version__.split(".")[2]),
     0,
 )
```

### Comparing `icecube-skyreader-1.1.0/skyreader/event_metadata.py` & `icecube-skyreader-1.2.0/skyreader/event_metadata.py`

 * *Files identical despite different names*

### Comparing `icecube-skyreader-1.1.0/skyreader/plot/plotting_tools.py` & `icecube-skyreader-1.2.0/skyreader/plot/plotting_tools.py`

 * *Files identical despite different names*

### Comparing `icecube-skyreader-1.1.0/skyreader/result.py` & `icecube-skyreader-1.2.0/skyreader/result.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,49 +172,31 @@
         )
 
     def isclose_pixel(
         self,
         sre_pix: np.ndarray,
         ore_pix: np.ndarray,
         equal_nan: bool,
-        do_disqualify_zero_energy_pixels: bool,  # TODO: remove?
         rtol_per_field: Dict[str, float],
     ) -> Tuple[List[float], List[bool]]:
         """Get the diff float-values and test truth-values for the 2 pixel-
         data.
 
         The datapoints are compared face-to-face (zipped).
-
-        If `do_disqualify_zero_energy_pixels=True` there's an
-        invalid datapoint value in either array, all "require close"
-        datapoints are considered (vacuously) close enough. # TODO: remove?
         """
         diff_vals = []
         test_vals = []
 
-        # is one of the pixel-datapoints is "so bad" it has
-        # disqualified all the other "require_close" datapoints?
-        is_pixel_disqualified = False  # TODO: remove?
-        if do_disqualify_zero_energy_pixels:  # TODO: remove?
-            is_pixel_disqualified = any(
-                sre_pix[self.PIXEL_FIELDS.index(f)] == 0.0
-                or ore_pix[self.PIXEL_FIELDS.index(f)] == 0.0
-                for f in ZERO_MAKES_FIELD_ALWAYS_ISCLOSE
-            )
-
         for s_val, o_val, field in zip(sre_pix, ore_pix, self.PIXEL_FIELDS):
             s_val, o_val = float(s_val), float(o_val)
 
-            # CASE 1: a disqualified-pixel "require close" datapoint
-            if field in rtol_per_field and is_pixel_disqualified:
-                diff, test = float("nan"), True  # vacuously true
-            # CASE 2: a "require close" datapoint (not disqualified-pixel)
-            elif field in rtol_per_field:
+            # CASE: a "require close" datapoint
+            if field in rtol_per_field:
                 diff, test = self.isclose_datapoint(s_val, o_val, field, equal_nan, rtol_per_field)
-            # CASE 3: a "require equal" datapoint
+            # CASE: a "require equal" datapoint
             else:
                 diff, test = s_val - o_val, s_val == o_val
 
             diff_vals.append(diff)
             test_vals.append(test)
 
         return diff_vals, test_vals
@@ -243,28 +225,27 @@
         else:
             self.logger.warning("Metadata doesn't seem to exist and will not be used for plotting.")
             return EventMetadata(0, 0, '', 0, False)
 
     def isclose_nside(self,
         other: "SkyScanResult",
         equal_nan: bool,
-        do_disqualify_zero_energy_pixels: bool,  # TODO: remove?
         rtol_per_field: Dict[str, float],
         nside: str,
     ) -> Tuple[bool, List[Tuple[Tuple[Any, ...], Tuple[Any, ...], Tuple[float, ...], Tuple[bool, ...]]]]:
         """Get whether the two nside's pixels are all "close"."""
         # zip-iterate each pixel-data
         nside_diffs = []
         for sre_pix, ore_pix in it.zip_longest(
             self.result.get(nside, []),  # empty-list -> fillvalue
             other.result.get(nside, []),  # empty-list -> fillvalue
             fillvalue=np.full((len(self.PIXEL_FIELDS),), np.nan),  # 1 vector
         ):
             diff_vals, test_vals = self.isclose_pixel(
-                sre_pix, ore_pix, equal_nan, do_disqualify_zero_energy_pixels, rtol_per_field
+                sre_pix, ore_pix, equal_nan, rtol_per_field
             )
             pix_diff = (
                 tuple(sre_pix.tolist()),
                 tuple(ore_pix.tolist()),
                 tuple(diff_vals),  # diff float-value
                 tuple(test_vals),  # test truth-value
             )
@@ -292,34 +273,28 @@
         return all(nside_equal.values()) and all(nside_close.values()), nside_diffs
 
     def is_close(
         self,
         other: "SkyScanResult",
         equal_nan: bool = True,
         dump_json_diff: Optional[Path] = None,
-        do_disqualify_zero_energy_pixels: bool = False,  # TODO: remove?
         rtol_per_field: Optional[Dict[str, float]] = None,
     ) -> bool:
         """Checks if two results are close by requiring strict equality on
         pixel indices and close condition on numeric results.
 
         Args:
             `other`
                 the instance to compare
             `equal_nan`
                 whether to let `nan == nan` be True
                 (default: `True`)
             `dump_json_diff`
                 get a json file containing every comparison at the pixel-data level
                 (default: `None`)
-            `do_disqualify_zero_energy_pixels`
-                If `do_disqualify_zero_energy_pixels=True` and there's an
-                invalid datapoint value in either array, all "require close"
-                datapoints are considered (vacuously) close enough. # TODO: remove?
-                (default: `False`)
             `rtol_per_field`
                 a mapping of each field to a rtol value
                 (default: `DEFAULT_RTOL_PER_FIELD`)
 
         Returns:
             bool: True if `other` and `self` are close
         """
@@ -331,15 +306,15 @@
 
         # now check individual nside-iterations
         for nside in sorted(self.result.keys() & other.result.keys(), reverse=True):
             self.logger.info(f"Comparing for nside={nside}")
             # Q: why aren't we using np.array_equal and np.allclose?
             # A: we want detailed pixel-level diffs w/out repeating detailed code
             close[nside], diffs[nside] = self.isclose_nside(
-                other, equal_nan, do_disqualify_zero_energy_pixels, rtol_per_field, nside
+                other, equal_nan, rtol_per_field, nside
             )
 
         # finish up
         self.logger.info(f"Comparison result: {close}")
 
         if dump_json_diff:
             with open(dump_json_diff, "w") as f:
```

