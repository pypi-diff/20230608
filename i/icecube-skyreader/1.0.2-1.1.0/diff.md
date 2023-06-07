# Comparing `tmp/icecube-skyreader-1.0.2.tar.gz` & `tmp/icecube-skyreader-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icecube-skyreader-1.0.2.tar", last modified: Thu May  4 17:43:34 2023, max compression
+gzip compressed data, was "icecube-skyreader-1.1.0.tar", last modified: Wed Jun  7 22:08:18 2023, max compression
```

## Comparing `icecube-skyreader-1.0.2.tar` & `icecube-skyreader-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:43:34.789717 icecube-skyreader-1.0.2/
--rw-r--r--   0 root         (0) root         (0)     1085 2023-05-04 17:43:30.000000 icecube-skyreader-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1987 2023-05-04 17:43:34.789717 icecube-skyreader-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1025 2023-05-04 17:43:30.000000 icecube-skyreader-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:43:34.785717 icecube-skyreader-1.0.2/icecube_skyreader.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1987 2023-05-04 17:43:34.000000 icecube-skyreader-1.0.2/icecube_skyreader.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      389 2023-05-04 17:43:34.000000 icecube-skyreader-1.0.2/icecube_skyreader.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 17:43:34.000000 icecube-skyreader-1.0.2/icecube_skyreader.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      120 2023-05-04 17:43:34.000000 icecube-skyreader-1.0.2/icecube_skyreader.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-04 17:43:34.000000 icecube-skyreader-1.0.2/icecube_skyreader.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1762 2023-05-04 17:43:34.789717 icecube-skyreader-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       76 2023-05-04 17:43:30.000000 icecube-skyreader-1.0.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:43:34.789717 icecube-skyreader-1.0.2/skyreader/
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-04 17:43:31.000000 icecube-skyreader-1.0.2/skyreader/__init__.py
--rw-r--r--   0 root         (0) root         (0)      915 2023-05-04 17:43:30.000000 icecube-skyreader-1.0.2/skyreader/event_metadata.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:43:34.789717 icecube-skyreader-1.0.2/skyreader/plot/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:43:30.000000 icecube-skyreader-1.0.2/skyreader/plot/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9057 2023-05-04 17:43:30.000000 icecube-skyreader-1.0.2/skyreader/plot/plotting_tools.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:43:30.000000 icecube-skyreader-1.0.2/skyreader/py.typed
--rw-r--r--   0 root         (0) root         (0)    47027 2023-05-04 17:43:30.000000 icecube-skyreader-1.0.2/skyreader/result.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 22:08:18.950540 icecube-skyreader-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)     1085 2023-06-07 22:08:16.000000 icecube-skyreader-1.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1987 2023-06-07 22:08:18.950540 icecube-skyreader-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1025 2023-06-07 22:08:16.000000 icecube-skyreader-1.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 22:08:18.950540 icecube-skyreader-1.1.0/icecube_skyreader.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1987 2023-06-07 22:08:18.000000 icecube-skyreader-1.1.0/icecube_skyreader.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      389 2023-06-07 22:08:18.000000 icecube-skyreader-1.1.0/icecube_skyreader.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 22:08:18.000000 icecube-skyreader-1.1.0/icecube_skyreader.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      120 2023-06-07 22:08:18.000000 icecube-skyreader-1.1.0/icecube_skyreader.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-07 22:08:18.000000 icecube-skyreader-1.1.0/icecube_skyreader.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1762 2023-06-07 22:08:18.950540 icecube-skyreader-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       76 2023-06-07 22:08:16.000000 icecube-skyreader-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 22:08:18.950540 icecube-skyreader-1.1.0/skyreader/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-07 22:08:16.000000 icecube-skyreader-1.1.0/skyreader/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      915 2023-06-07 22:08:16.000000 icecube-skyreader-1.1.0/skyreader/event_metadata.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 22:08:18.950540 icecube-skyreader-1.1.0/skyreader/plot/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 22:08:16.000000 icecube-skyreader-1.1.0/skyreader/plot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9057 2023-06-07 22:08:16.000000 icecube-skyreader-1.1.0/skyreader/plot/plotting_tools.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 22:08:16.000000 icecube-skyreader-1.1.0/skyreader/py.typed
+-rw-r--r--   0 root         (0) root         (0)    48327 2023-06-07 22:08:16.000000 icecube-skyreader-1.1.0/skyreader/result.py
```

### Comparing `icecube-skyreader-1.0.2/LICENSE` & `icecube-skyreader-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `icecube-skyreader-1.0.2/PKG-INFO` & `icecube-skyreader-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icecube-skyreader
-Version: 1.0.2
+Version: 1.1.0
 Summary: An API for Results Produced by SkyDriver & the Skymap Scanner
 Home-page: https://github.com/icecube/skyreader
 Download-URL: https://pypi.org/project/icecube-skyreader/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/icecube/skyreader/issues
```

### Comparing `icecube-skyreader-1.0.2/README.md` & `icecube-skyreader-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `icecube-skyreader-1.0.2/icecube_skyreader.egg-info/PKG-INFO` & `icecube-skyreader-1.1.0/icecube_skyreader.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icecube-skyreader
-Version: 1.0.2
+Version: 1.1.0
 Summary: An API for Results Produced by SkyDriver & the Skymap Scanner
 Home-page: https://github.com/icecube/skyreader
 Download-URL: https://pypi.org/project/icecube-skyreader/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/icecube/skyreader/issues
```

### Comparing `icecube-skyreader-1.0.2/setup.cfg` & `icecube-skyreader-1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `icecube-skyreader-1.0.2/skyreader/__init__.py` & `icecube-skyreader-1.1.0/skyreader/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,14 @@
 # version is a human-readable version number.
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
-__version__ = "1.0.2"
+__version__ = "1.1.0"
 version_info = (
     int(__version__.split(".")[0]),
     int(__version__.split(".")[1]),
     int(__version__.split(".")[2]),
     0,
 )
```

### Comparing `icecube-skyreader-1.0.2/skyreader/event_metadata.py` & `icecube-skyreader-1.1.0/skyreader/event_metadata.py`

 * *Files identical despite different names*

### Comparing `icecube-skyreader-1.0.2/skyreader/plot/plotting_tools.py` & `icecube-skyreader-1.1.0/skyreader/plot/plotting_tools.py`

 * *Files identical despite different names*

### Comparing `icecube-skyreader-1.0.2/skyreader/result.py` & `icecube-skyreader-1.1.0/skyreader/result.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,59 @@
 """For encapsulating the results of an event scan in a single instance."""
 
 # fmt: off
 # pylint: skip-file
-# mypy: ignore-errors
 # flake8: noqa
 
 
 import io
 import itertools as it
 import json
 import logging
 import pickle
 from functools import cached_property
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple, TypedDict, Union
 
-import healpy
-import matplotlib
-import meander
+import healpy  # type: ignore[import]
+import matplotlib  # type: ignore[import]
+import meander  # type: ignore[import]
 import numpy as np
-import pandas as pd
-from astropy.io import ascii
+import pandas as pd  # type: ignore[import]
+from astropy.io import ascii  # type: ignore[import]
+from matplotlib import patheffects
 from matplotlib import pyplot as plt
-from matplotlib import text, patheffects
+from matplotlib import text
 
 from .event_metadata import EventMetadata
+from .plot.plotting_tools import (
+    DecFormatter,
+    RaFormatter,
+    format_fits_header,
+    hp_ticklabels,
+    plot_catalog,
+)
+
+###############################################################################
+# CONSTANTS
+
+
+# bookkeeping for comparing values
+DEFAULT_RTOL_PER_FIELD = {  # w/ rtol values
+    # any field not here is assumed to require '==' for comparison
+    "llh": 1e-4,
+    "E_in": 1e-2,
+    "E_tot": 1e-2,
+}
+ZERO_MAKES_FIELD_ALWAYS_ISCLOSE = [
+    # if a pixel field's val is 0, then that datapoint is "isclose" to any value
+    "E_in",
+    "E_tot",
+]
 
-from .plot.plotting_tools import format_fits_header, hp_ticklabels, plot_catalog, DecFormatter, RaFormatter
 
 ###############################################################################
 # DATA TYPES
 
 
 class PyDictNSidePixels(TypedDict):
     columns: List[str]
@@ -38,22 +61,14 @@
     data: List[List[Union[int, float]]]
 
 
 PyDictResult = Dict[str, PyDictNSidePixels]
 
 
 ###############################################################################
-# EXCPETIONS
-
-
-class InvalidPixelValueError(Exception):
-    """Raised when a pixel-value is illegal."""
-
-
-###############################################################################
 # MAIN CLASS
 
 class SkyScanResult:
     """This class parses a nsides_dict and stores the relevant numeric result
     of the scan. Ideally it should serve as the basic data structure for
     plotting / processing / transmission of the scan result.
 
@@ -73,14 +88,15 @@
 
     TODO: implement FITS output.
     """
 
     PIXEL_TYPE = np.dtype(
         [("index", int), ("llh", float), ("E_in", float), ("E_tot", float)]
     )
+    PIXEL_FIELDS: Tuple[str, ...] = PIXEL_TYPE.names  # type: ignore[assignment]
     ATOL = 1.0e-8  # 1.0e-8 is the default used by np.isclose()
 
     def __init__(self, result: Dict[str, np.ndarray]):
         self.logger = logging.getLogger(__name__)
 
         # validate result data
         if not isinstance(result, dict):
@@ -98,26 +114,15 @@
                     f"should be {self.PIXEL_TYPE}"
                 )
         self.result = result
         self.nsides = sorted([self.parse_nside(key) for key in self.result])
 
         self.logger.debug(f"Metadata for this result: {[self.result[_].dtype.metadata for _ in self.result]}")
 
-        # bookkeeping for comparing values
-        self.require_close = {  # w/ rtol values
-            # any field not here is assumed to require '==' for comparison
-            "llh": 1e-4,
-            "E_in": 1e-2,
-            "E_tot": 1e-2,
-        }
-        self.cannot_be_zero_fields = [
-            # if field's val is 0, then all the pixel's numerical datapoints are "isclose"
-            "E_in",
-            "E_tot",
-        ]
+
 
     """
     Comparison operators and methods
     """
 
     def __eq__(self, other: object) -> bool:
         """Are the two instance's result lists strictly equal?"""
@@ -128,49 +133,55 @@
         # NOTE: will return false if NaN are present
         # np.array_equal() supports `equal_nan` option only from version 1.19
         return all(
             np.array_equal(self.result[nside], other.result[nside])
             for nside in self.result
         )
 
-    def is_close_datapoint(
-        self, s_val: float, o_val: float, field: str, equal_nan: bool
+    def isclose_datapoint(
+        self,
+        s_val: float,
+        o_val: float,
+        field: str,
+        equal_nan: bool,
+        rtol_per_field: Dict[str, float],
     ) -> Tuple[float, bool]:
         """Get the diff float-value and test truth-value for the 2 pixel
         datapoints."""
-        if field not in self.require_close:
+        if field not in rtol_per_field:
             raise ValueError(
                 f"Datapoint field ({field}) cannot be compared by "
                 f"'is_close_datapoint()', must use '=='"
             )
-        if field in self.cannot_be_zero_fields and (s_val == 0.0 or o_val == 0.0):
-            raise InvalidPixelValueError(f"field={field}, values={(s_val, o_val)}")
+        if field in ZERO_MAKES_FIELD_ALWAYS_ISCLOSE and (s_val == 0.0 or o_val == 0.0):
+            return float("nan"), True
         try:
             rdiff = (abs(s_val - o_val) - self.ATOL) / abs(o_val)  # used by np.isclose
         except ZeroDivisionError:
             rdiff = float("inf")
         return (
             rdiff,
             bool(
                 np.isclose(
                     s_val,
                     o_val,
                     equal_nan=equal_nan,
-                    rtol=self.require_close[field],
+                    rtol=rtol_per_field[field],
                     atol=self.ATOL,
                 )
             ),
         )
 
-    def diff_pixel_data(
+    def isclose_pixel(
         self,
         sre_pix: np.ndarray,
         ore_pix: np.ndarray,
         equal_nan: bool,
         do_disqualify_zero_energy_pixels: bool,  # TODO: remove?
+        rtol_per_field: Dict[str, float],
     ) -> Tuple[List[float], List[bool]]:
         """Get the diff float-values and test truth-values for the 2 pixel-
         data.
 
         The datapoints are compared face-to-face (zipped).
 
         If `do_disqualify_zero_energy_pixels=True` there's an
@@ -181,31 +192,28 @@
         test_vals = []
 
         # is one of the pixel-datapoints is "so bad" it has
         # disqualified all the other "require_close" datapoints?
         is_pixel_disqualified = False  # TODO: remove?
         if do_disqualify_zero_energy_pixels:  # TODO: remove?
             is_pixel_disqualified = any(
-                sre_pix[self.PIXEL_TYPE.names.index(f)] == 0.0
-                or ore_pix[self.PIXEL_TYPE.names.index(f)] == 0.0
-                for f in self.cannot_be_zero_fields
+                sre_pix[self.PIXEL_FIELDS.index(f)] == 0.0
+                or ore_pix[self.PIXEL_FIELDS.index(f)] == 0.0
+                for f in ZERO_MAKES_FIELD_ALWAYS_ISCLOSE
             )
 
-        for s_val, o_val, field in zip(sre_pix, ore_pix, self.PIXEL_TYPE.names):
+        for s_val, o_val, field in zip(sre_pix, ore_pix, self.PIXEL_FIELDS):
             s_val, o_val = float(s_val), float(o_val)
 
             # CASE 1: a disqualified-pixel "require close" datapoint
-            if field in self.require_close and is_pixel_disqualified:
+            if field in rtol_per_field and is_pixel_disqualified:
                 diff, test = float("nan"), True  # vacuously true
             # CASE 2: a "require close" datapoint (not disqualified-pixel)
-            elif field in self.require_close:
-                try:
-                    diff, test = self.is_close_datapoint(s_val, o_val, field, equal_nan)
-                except InvalidPixelValueError:
-                    diff, test = float("nan"), True
+            elif field in rtol_per_field:
+                diff, test = self.isclose_datapoint(s_val, o_val, field, equal_nan, rtol_per_field)
             # CASE 3: a "require equal" datapoint
             else:
                 diff, test = s_val - o_val, s_val == o_val
 
             diff_vals.append(diff)
             test_vals.append(test)
 
@@ -232,81 +240,107 @@
                 first_metadata['mjd'],
                 first_metadata.get('is_real_event', False),  # assume simulated event
             )
         else:
             self.logger.warning("Metadata doesn't seem to exist and will not be used for plotting.")
             return EventMetadata(0, 0, '', 0, False)
 
+    def isclose_nside(self,
+        other: "SkyScanResult",
+        equal_nan: bool,
+        do_disqualify_zero_energy_pixels: bool,  # TODO: remove?
+        rtol_per_field: Dict[str, float],
+        nside: str,
+    ) -> Tuple[bool, List[Tuple[Tuple[Any, ...], Tuple[Any, ...], Tuple[float, ...], Tuple[bool, ...]]]]:
+        """Get whether the two nside's pixels are all "close"."""
+        # zip-iterate each pixel-data
+        nside_diffs = []
+        for sre_pix, ore_pix in it.zip_longest(
+            self.result.get(nside, []),  # empty-list -> fillvalue
+            other.result.get(nside, []),  # empty-list -> fillvalue
+            fillvalue=np.full((len(self.PIXEL_FIELDS),), np.nan),  # 1 vector
+        ):
+            diff_vals, test_vals = self.isclose_pixel(
+                sre_pix, ore_pix, equal_nan, do_disqualify_zero_energy_pixels, rtol_per_field
+            )
+            pix_diff = (
+                tuple(sre_pix.tolist()),
+                tuple(ore_pix.tolist()),
+                tuple(diff_vals),  # diff float-value
+                tuple(test_vals),  # test truth-value
+            )
+            for vals in pix_diff:
+                self.logger.debug(f"{nside}: {vals}")
+            nside_diffs.append(pix_diff)
+
+        # aggregate test-truth values
+        nside_equal = {
+            field: all(d[3][self.PIXEL_FIELDS.index(field)] for d in nside_diffs)
+            for field in set(self.PIXEL_FIELDS) - set(rtol_per_field)
+        }
+        nside_close = {
+            field: all(d[3][self.PIXEL_FIELDS.index(field)] for d in nside_diffs)
+            for field in rtol_per_field
+        }
+
+        # log results (test-truth values)
+        if not all(nside_equal.values()):
+            self.logger.info(f"Mismatched pixel indices for nside={nside}")
+        if not all(nside_close.values()):
+            self.logger.info(f"Mismatched numerical results for nside={nside}")
+            self.logger.debug(f"{nside_close}")
+
+        return all(nside_equal.values()) and all(nside_close.values()), nside_diffs
+
     def is_close(
         self,
         other: "SkyScanResult",
         equal_nan: bool = True,
         dump_json_diff: Optional[Path] = None,
         do_disqualify_zero_energy_pixels: bool = False,  # TODO: remove?
+        rtol_per_field: Optional[Dict[str, float]] = None,
     ) -> bool:
         """Checks if two results are close by requiring strict equality on
         pixel indices and close condition on numeric results.
 
-        Optionally, pass a `Path` for `dump_json_diff` to get a json
-        file containing every diff at the pixel-data level.
+        Args:
+            `other`
+                the instance to compare
+            `equal_nan`
+                whether to let `nan == nan` be True
+                (default: `True`)
+            `dump_json_diff`
+                get a json file containing every comparison at the pixel-data level
+                (default: `None`)
+            `do_disqualify_zero_energy_pixels`
+                If `do_disqualify_zero_energy_pixels=True` and there's an
+                invalid datapoint value in either array, all "require close"
+                datapoints are considered (vacuously) close enough. # TODO: remove?
+                (default: `False`)
+            `rtol_per_field`
+                a mapping of each field to a rtol value
+                (default: `DEFAULT_RTOL_PER_FIELD`)
+
+        Returns:
+            bool: True if `other` and `self` are close
         """
+        if not rtol_per_field:
+            rtol_per_field = DEFAULT_RTOL_PER_FIELD
+
         close: Dict[str, bool] = {}  # one bool for each nside value
         diffs: Dict[str, list] = {}  # (~4x size of self.results) w/ per-pixel info
 
         # now check individual nside-iterations
         for nside in sorted(self.result.keys() & other.result.keys(), reverse=True):
             self.logger.info(f"Comparing for nside={nside}")
-
             # Q: why aren't we using np.array_equal and np.allclose?
             # A: we want detailed pixel-level diffs w/out repeating detailed code
-
-            # zip-iterate each pixel-data
-            nside_diffs = []
-            for sre_pix, ore_pix in it.zip_longest(
-                self.result.get(nside, []),  # empty-list -> fillvalue
-                other.result.get(nside, []),  # empty-list -> fillvalue
-                fillvalue=np.full((len(self.PIXEL_TYPE.names),), np.nan),  # 1 vector
-            ):
-                diff_vals, test_vals = self.diff_pixel_data(
-                    sre_pix, ore_pix, equal_nan, do_disqualify_zero_energy_pixels
-                )
-                pix_diff = [
-                    tuple(sre_pix.tolist()),
-                    tuple(ore_pix.tolist()),
-                    tuple(diff_vals),  # diff float-value
-                    tuple(test_vals),  # test truth-value
-                ]
-                for vals in pix_diff:
-                    self.logger.debug(f"{nside}: {vals}")
-                nside_diffs.append(pix_diff)
-
-            if dump_json_diff:  # can be a lot of data, so only save it if we're dumping
-                diffs[nside] = nside_diffs
-
-            # aggregate test-truth values
-            nside_equal = {
-                field: all(
-                    d[3][self.PIXEL_TYPE.names.index(field)] for d in nside_diffs
-                )
-                for field in set(self.PIXEL_TYPE.names) - set(self.require_close)
-            }
-            nside_close = {
-                field: all(
-                    d[3][self.PIXEL_TYPE.names.index(field)] for d in nside_diffs
-                )
-                for field in self.require_close
-            }
-            close[nside] = all(nside_equal.values()) and all(nside_close.values())
-
-            # log results (test-truth values)
-            if not all(nside_equal.values()):
-                self.logger.info(f"Mismatched pixel indices for nside={nside}")
-            if not all(nside_close.values()):
-                self.logger.info(f"Mismatched numerical results for nside={nside}")
-                self.logger.debug(f"{nside_close}")
+            close[nside], diffs[nside] = self.isclose_nside(
+                other, equal_nan, do_disqualify_zero_energy_pixels, rtol_per_field, nside
+            )
 
         # finish up
         self.logger.info(f"Comparison result: {close}")
 
         if dump_json_diff:
             with open(dump_json_diff, "w") as f:
                 self.logger.info(f"Writing diff to {dump_json_diff}...")
@@ -361,37 +395,47 @@
         if "header" not in npz:
             for key in npz.keys():
                 result[key] = npz[key]
         else:
             h = npz["header"]
             for v in h:
                 key = cls.format_nside(v['nside'])
-                _dtype = np.dtype(npz[key].dtype, metadata={k:value for k, value in zip(h.dtype.fields.keys(), v)})
+                _dtype = np.dtype(
+                    npz[key].dtype,
+                    metadata={k:value for k, value in zip(h.dtype.fields.keys(), v)},  # type: ignore[call-overload]
+                )
                 result[key] = np.array(list(npz[key]), dtype=_dtype)
         return cls(result=result)
 
     def to_npz(
         self,
         event_metadata: EventMetadata,
         output_dir: Union[str, Path, None] = None,
     ) -> Path:
         """Save to .npz file."""
         filename = self.get_filename(event_metadata, '.npz', output_dir)
 
         try:
             metadata_dtype = np.dtype(
-                [(k, type(v)) if not isinstance(v, str) else (k, f"U{len(v)}")
-                 for k, v in next(iter(self.result.values())).dtype.metadata.items()],
-                )
-            h = np.array([tuple(self.result[k].dtype.metadata[mk] for mk in metadata_dtype.fields)
-                           for k in self.result],
-                         dtype=metadata_dtype)
+                [
+                    (k, type(v)) if not isinstance(v, str) else (k, f"U{len(v)}")
+                    for k, v in next(iter(self.result.values())).dtype.metadata.items()
+                ],
+            )
+            h = np.array(
+                [
+                    tuple(self.result[k].dtype.metadata[mk] for mk in metadata_dtype.fields)  # type: ignore[union-attr]
+                    for k in self.result
+                ],
+                dtype=metadata_dtype,
+            )
             np.savez(filename, header=h, **self.result)
         except (TypeError, AttributeError):
             np.savez(filename, **self.result)
+
         return Path(filename)
 
     """
     JSON input / output
     """
 
     @classmethod
@@ -424,32 +468,35 @@
 
         for nside, pydict_nside_pixels in pydict.items():
             # validate keys
             if set(pydict_nside_pixels.keys()) != {'columns', 'metadata', 'data'}:
                 raise ValueError(f"PyDictResult entry has extra/missing keys: {pydict_nside_pixels.keys()}")
 
             # check 'columns'
-            if pydict_nside_pixels['columns'] != list(cls.PIXEL_TYPE.names):  # type: ignore[arg-type]
+            if pydict_nside_pixels['columns'] != list(cls.PIXEL_FIELDS):
                 raise ValueError(
                     f"PyDictResult entry has invalid 'columns' entry "
-                    f"({pydict_nside_pixels['columns']}) should be {list(cls.PIXEL_TYPE.names)}"  # type: ignore[arg-type]
+                    f"({pydict_nside_pixels['columns']}) should be {list(cls.PIXEL_FIELDS)}"
                 )
 
             # check 'metadata'
             try:
                 if pydict_nside_pixels['metadata']['nside'] != cls.parse_nside(nside):
                     raise ValueError(
                         f"PyDictResult entry has incorrect 'metadata'.'nside' value: "
                         f"{pydict_nside_pixels['metadata']['nside']} should be {cls.parse_nside(nside)}"
                     )
             except (KeyError, TypeError) as e:
                 raise ValueError("PyDictResult entry has missing key 'nside'") from e
 
             # read/convert
-            _dtype = np.dtype(cls.PIXEL_TYPE, metadata=pydict_nside_pixels['metadata'])
+            _dtype = np.dtype(
+                cls.PIXEL_TYPE,
+                metadata=pydict_nside_pixels['metadata'],  # type: ignore[call-overload]
+            )
             result_nside_pixels = np.zeros(len(pydict_nside_pixels['data']), dtype=_dtype)
             for i, pix_4list in enumerate(sorted(pydict_nside_pixels['data'], key=lambda x: x[0])):
                 result_nside_pixels[i] = tuple(pix_4list)
 
             result[nside] = result_nside_pixels
 
         return cls(result)
@@ -485,22 +532,21 @@
                     ],
                     ...
                 ]
             },
             ...
         }
         """
-        pydict = {}
+        pydict: PyDictResult = {}
         for nside in self.result:
             df = pd.DataFrame(
                 self.result[nside],
                 columns=list(self.result[nside].dtype.names),
             )
-            pydict[nside] = df.to_dict(orient='split')
-            pydict[nside].pop('index')  # index is not necessary
+            pydict[nside] = {k:v for k,v in df.to_dict(orient='split').items() if k != 'index'}  # type: ignore[assignment]
             pydict[nside]['metadata'] = dict(self.result[nside].dtype.metadata)
         return pydict
 
     """
     Querying
     """
```

