# Comparing `tmp/bw_temporalis-0.6.tar.gz` & `tmp/bw_temporalis-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bw_temporalis-0.6.tar", last modified: Mon May  8 08:49:50 2023, max compression
+gzip compressed data, was "bw_temporalis-0.7.tar", last modified: Thu Jun  8 08:56:22 2023, max compression
```

## Comparing `bw_temporalis-0.6.tar` & `bw_temporalis-0.7.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-05-08 08:49:50.739924 bw_temporalis-0.6/
--rw-r--r--   0 chrismutel   (501) staff       (20)     1456 2023-04-23 13:14:37.000000 bw_temporalis-0.6/LICENSE
--rw-r--r--   0 chrismutel   (501) staff       (20)       30 2023-04-23 13:14:37.000000 bw_temporalis-0.6/MANIFEST.in
--rw-r--r--   0 chrismutel   (501) staff       (20)     3026 2023-05-08 08:49:50.739986 bw_temporalis-0.6/PKG-INFO
--rw-r--r--   0 chrismutel   (501) staff       (20)     1955 2023-04-23 13:14:37.000000 bw_temporalis-0.6/README.md
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-05-08 08:49:50.737599 bw_temporalis-0.6/bw_temporalis/
--rw-r--r--   0 chrismutel   (501) staff       (20)        4 2023-05-08 08:40:52.000000 bw_temporalis-0.6/bw_temporalis/VERSION
--rw-r--r--   0 chrismutel   (501) staff       (20)      608 2023-05-01 16:31:17.000000 bw_temporalis-0.6/bw_temporalis/__init__.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     3287 2023-05-01 16:31:04.000000 bw_temporalis-0.6/bw_temporalis/convolution.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     8241 2023-05-08 08:37:38.000000 bw_temporalis-0.6/bw_temporalis/lca.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-05-08 08:49:50.736585 bw_temporalis-0.6/bw_temporalis/lcia/
--rw-r--r--   0 chrismutel   (501) staff       (20)       60 2023-04-30 15:06:21.000000 bw_temporalis-0.6/bw_temporalis/lcia/__init__.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     4752 2023-04-30 15:06:26.000000 bw_temporalis-0.6/bw_temporalis/lcia/climate.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     8862 2023-05-03 18:06:46.000000 bw_temporalis-0.6/bw_temporalis/temporal_distribution.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     7106 2023-05-07 20:04:42.000000 bw_temporalis-0.6/bw_temporalis/timeline.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     9820 2023-05-07 20:05:01.000000 bw_temporalis-0.6/bw_temporalis/utils.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-05-08 08:49:50.738350 bw_temporalis-0.6/bw_temporalis.egg-info/
--rw-r--r--   0 chrismutel   (501) staff       (20)     3026 2023-05-08 08:49:50.000000 bw_temporalis-0.6/bw_temporalis.egg-info/PKG-INFO
--rw-r--r--   0 chrismutel   (501) staff       (20)      737 2023-05-08 08:49:50.000000 bw_temporalis-0.6/bw_temporalis.egg-info/SOURCES.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-05-08 08:49:50.000000 bw_temporalis-0.6/bw_temporalis.egg-info/dependency_links.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-04-26 11:46:09.000000 bw_temporalis-0.6/bw_temporalis.egg-info/not-zip-safe
--rw-r--r--   0 chrismutel   (501) staff       (20)      174 2023-05-08 08:49:50.000000 bw_temporalis-0.6/bw_temporalis.egg-info/requires.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)       37 2023-05-08 08:49:50.000000 bw_temporalis-0.6/bw_temporalis.egg-info/top_level.txt
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-05-08 08:49:50.736822 bw_temporalis-0.6/docs/
--rw-r--r--   0 chrismutel   (501) staff       (20)     1151 2023-04-23 13:14:37.000000 bw_temporalis-0.6/docs/conf.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-05-08 08:49:50.737382 bw_temporalis-0.6/examples/
--rw-r--r--   0 chrismutel   (501) staff       (20)     1500 2023-04-26 18:20:47.000000 bw_temporalis-0.6/examples/__init__.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     4350 2023-04-26 18:20:47.000000 bw_temporalis-0.6/examples/ia.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     6149 2023-04-27 11:45:54.000000 bw_temporalis-0.6/examples/inv.py
--rw-r--r--   0 chrismutel   (501) staff       (20)       87 2023-04-23 13:14:37.000000 bw_temporalis-0.6/pyproject.toml
--rw-r--r--   0 chrismutel   (501) staff       (20)     1754 2023-05-08 08:49:50.740367 bw_temporalis-0.6/setup.cfg
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-05-08 08:49:50.739566 bw_temporalis-0.6/tests/
--rw-r--r--   0 chrismutel   (501) staff       (20)     8786 2023-04-30 15:06:08.000000 bw_temporalis-0.6/tests/test_convolution.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     8567 2023-04-27 11:45:54.000000 bw_temporalis-0.6/tests/test_fixtures.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     7855 2023-05-08 08:38:16.000000 bw_temporalis-0.6/tests/test_lca.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     5952 2023-05-08 08:37:38.000000 bw_temporalis-0.6/tests/test_td.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     4301 2023-05-07 20:05:01.000000 bw_temporalis-0.6/tests/test_timeline.py
--rw-r--r--   0 chrismutel   (501) staff       (20)    13141 2023-05-07 20:05:16.000000 bw_temporalis-0.6/tests/test_utils.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-06-08 08:56:22.552687 bw_temporalis-0.7/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1456 2023-04-23 13:14:37.000000 bw_temporalis-0.7/LICENSE
+-rw-r--r--   0 chrismutel   (501) staff       (20)       30 2023-04-23 13:14:37.000000 bw_temporalis-0.7/MANIFEST.in
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3399 2023-06-08 08:56:22.552743 bw_temporalis-0.7/PKG-INFO
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2328 2023-05-08 09:25:57.000000 bw_temporalis-0.7/README.md
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-06-08 08:56:22.549527 bw_temporalis-0.7/bw_temporalis/
+-rw-r--r--   0 chrismutel   (501) staff       (20)        4 2023-06-08 08:55:32.000000 bw_temporalis-0.7/bw_temporalis/VERSION
+-rw-r--r--   0 chrismutel   (501) staff       (20)      956 2023-06-08 05:53:02.000000 bw_temporalis-0.7/bw_temporalis/__init__.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3287 2023-05-01 16:31:04.000000 bw_temporalis-0.7/bw_temporalis/convolution.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     8872 2023-06-07 19:16:17.000000 bw_temporalis-0.7/bw_temporalis/lca.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-06-08 08:56:22.548501 bw_temporalis-0.7/bw_temporalis/lcia/
+-rw-r--r--   0 chrismutel   (501) staff       (20)       60 2023-04-30 15:06:21.000000 bw_temporalis-0.7/bw_temporalis/lcia/__init__.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4752 2023-04-30 15:06:26.000000 bw_temporalis-0.7/bw_temporalis/lcia/climate.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)    15687 2023-06-08 06:22:33.000000 bw_temporalis-0.7/bw_temporalis/temporal_distribution.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     7106 2023-05-07 20:04:42.000000 bw_temporalis-0.7/bw_temporalis/timeline.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     9817 2023-06-08 08:53:29.000000 bw_temporalis-0.7/bw_temporalis/utils.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-06-08 08:56:22.550376 bw_temporalis-0.7/bw_temporalis.egg-info/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3399 2023-06-08 08:56:22.000000 bw_temporalis-0.7/bw_temporalis.egg-info/PKG-INFO
+-rw-r--r--   0 chrismutel   (501) staff       (20)      798 2023-06-08 08:56:22.000000 bw_temporalis-0.7/bw_temporalis.egg-info/SOURCES.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-06-08 08:56:22.000000 bw_temporalis-0.7/bw_temporalis.egg-info/dependency_links.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-04-26 11:46:09.000000 bw_temporalis-0.7/bw_temporalis.egg-info/not-zip-safe
+-rw-r--r--   0 chrismutel   (501) staff       (20)      174 2023-06-08 08:56:22.000000 bw_temporalis-0.7/bw_temporalis.egg-info/requires.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)       37 2023-06-08 08:56:22.000000 bw_temporalis-0.7/bw_temporalis.egg-info/top_level.txt
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-06-08 08:56:22.548705 bw_temporalis-0.7/docs/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1151 2023-04-23 13:14:37.000000 bw_temporalis-0.7/docs/conf.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-06-08 08:56:22.549251 bw_temporalis-0.7/examples/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1500 2023-04-26 18:20:47.000000 bw_temporalis-0.7/examples/__init__.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4350 2023-04-26 18:20:47.000000 bw_temporalis-0.7/examples/ia.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     6149 2023-04-27 11:45:54.000000 bw_temporalis-0.7/examples/inv.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)       87 2023-04-23 13:14:37.000000 bw_temporalis-0.7/pyproject.toml
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1754 2023-06-08 08:56:22.553117 bw_temporalis-0.7/setup.cfg
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-06-08 08:56:22.552448 bw_temporalis-0.7/tests/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     8786 2023-04-30 15:06:08.000000 bw_temporalis-0.7/tests/test_convolution.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     5887 2023-06-08 06:19:51.000000 bw_temporalis-0.7/tests/test_fixed_time_of_year.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     8567 2023-04-27 11:45:54.000000 bw_temporalis-0.7/tests/test_fixtures.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     7855 2023-05-08 08:38:16.000000 bw_temporalis-0.7/tests/test_lca.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4074 2023-06-08 05:36:01.000000 bw_temporalis-0.7/tests/test_serialization.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     5957 2023-06-01 06:27:17.000000 bw_temporalis-0.7/tests/test_td.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4301 2023-05-07 20:05:01.000000 bw_temporalis-0.7/tests/test_timeline.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)    13141 2023-05-07 20:05:16.000000 bw_temporalis-0.7/tests/test_utils.py
```

### Comparing `bw_temporalis-0.6/LICENSE` & `bw_temporalis-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.6/PKG-INFO` & `bw_temporalis-0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw_temporalis
-Version: 0.6
+Version: 0.7
 Summary: Revision of bw2temporalis for modern Brightway
 Home-page: https://github.com/brightway-lca/bw_temporalis
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: BSD-3-Clause
@@ -52,14 +52,18 @@
 
 You can install _bw_temporalis_ via [pip] from [PyPI]:
 
 ```console
 $ pip install bw_temporalis
 ```
 
+Currently Python 3.11 installations are broken as [scikit-network](https://scikit-network.readthedocs.io/en/latest/?badge=latest) doesn't have pre-built wheels and compilation fails. This [could be fixed soon](https://github.com/sknetwork-team/scikit-network/pull/558).
+
+You can also install using conda in the [cmutel channel](https://anaconda.org/cmutel/bw_temporalis).
+
 ## Contributing
 
 Contributions are very welcome.
 To learn more, see the [Contributor Guide].
 
 ## License
```

### Comparing `bw_temporalis-0.6/README.md` & `bw_temporalis-0.7/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -23,14 +23,18 @@
 
 You can install _bw_temporalis_ via [pip] from [PyPI]:
 
 ```console
 $ pip install bw_temporalis
 ```
 
+Currently Python 3.11 installations are broken as [scikit-network](https://scikit-network.readthedocs.io/en/latest/?badge=latest) doesn't have pre-built wheels and compilation fails. This [could be fixed soon](https://github.com/sknetwork-team/scikit-network/pull/558).
+
+You can also install using conda in the [cmutel channel](https://anaconda.org/cmutel/bw_temporalis).
+
 ## Contributing
 
 Contributions are very welcome.
 To learn more, see the [Contributor Guide].
 
 ## License
```

### Comparing `bw_temporalis-0.6/bw_temporalis/convolution.py` & `bw_temporalis-0.7/bw_temporalis/convolution.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.6/bw_temporalis/lca.py` & `bw_temporalis-0.7/bw_temporalis/lca.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 from collections import defaultdict
 from collections.abc import Iterable
 from datetime import datetime
 from heapq import heappop, heappush
 
 import bw2data as bd
 import numpy as np
@@ -165,15 +166,32 @@
                         (td * value).simplify(),
                         producer,
                     ),
                 )
         return timeline
 
     def _exchange_value(self, exchange):
+        from . import loader_registry
+
         td = exchange.data.get("temporal_distribution")
+        if isinstance(td, str) and "__loader__" in td:
+            data = json.loads(td)
+            try:
+                td = loader_registry[td["__loader__"]](data)
+            except KeyError:
+                raise KeyError(
+                    "Can't find correct loader {} in `loader_registry`".format(
+                        td["__loader__"]
+                    )
+                )
+        elif not (isinstance(td, TD) or td is None):
+            raise ValueError(
+                f"Can't understand value for `temporal_distribution` in exchange {exchange}"
+            )
+
         if td is None:
             return exchange.data["amount"]
         else:
             return td * exchange.data["amount"]
 
     def _exchange_iterator(self, input_id: int, output_id: int) -> list[ED]:
         inp = AD.get(AD.id == input_id)
```

### Comparing `bw_temporalis-0.6/bw_temporalis/lcia/climate.py` & `bw_temporalis-0.7/bw_temporalis/lcia/climate.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.6/bw_temporalis/timeline.py` & `bw_temporalis-0.7/bw_temporalis/timeline.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.6/bw_temporalis/utils.py` & `bw_temporalis-0.7/bw_temporalis/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     `date` values are uniformly spaced from `start` to `end`.
 
     For triangular distributions, `param` is the mode (optional), and should
     be given in the same reference system as `start` and `stop`. The `param`
     value should be in the same format as `start` and `end`, e.g.
     "2023-01-01".
 
-    For lognormal distributions, `param` is the standard deviation in relation
+    For normal distributions, `param` is the standard deviation in relation
     to a standardized distribution with mu = 0. `param` is not used for the uniform distribution.
 
     Raises
     ------
     ValueError
         If the input parameters prevent construction of valide `TemporalDistribution`.
```

### Comparing `bw_temporalis-0.6/bw_temporalis.egg-info/PKG-INFO` & `bw_temporalis-0.7/bw_temporalis.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw-temporalis
-Version: 0.6
+Version: 0.7
 Summary: Revision of bw2temporalis for modern Brightway
 Home-page: https://github.com/brightway-lca/bw_temporalis
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: BSD-3-Clause
@@ -52,14 +52,18 @@
 
 You can install _bw_temporalis_ via [pip] from [PyPI]:
 
 ```console
 $ pip install bw_temporalis
 ```
 
+Currently Python 3.11 installations are broken as [scikit-network](https://scikit-network.readthedocs.io/en/latest/?badge=latest) doesn't have pre-built wheels and compilation fails. This [could be fixed soon](https://github.com/sknetwork-team/scikit-network/pull/558).
+
+You can also install using conda in the [cmutel channel](https://anaconda.org/cmutel/bw_temporalis).
+
 ## Contributing
 
 Contributions are very welcome.
 To learn more, see the [Contributor Guide].
 
 ## License
```

### Comparing `bw_temporalis-0.6/bw_temporalis.egg-info/SOURCES.txt` & `bw_temporalis-0.7/bw_temporalis.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -19,12 +19,14 @@
 bw_temporalis.egg-info/PKG-INFO
 bw_temporalis.egg-info/SOURCES.txt
 bw_temporalis.egg-info/dependency_links.txt
 bw_temporalis.egg-info/not-zip-safe
 bw_temporalis.egg-info/requires.txt
 bw_temporalis.egg-info/top_level.txt
 tests/test_convolution.py
+tests/test_fixed_time_of_year.py
 tests/test_fixtures.py
 tests/test_lca.py
+tests/test_serialization.py
 tests/test_td.py
 tests/test_timeline.py
 tests/test_utils.py
```

### Comparing `bw_temporalis-0.6/docs/conf.py` & `bw_temporalis-0.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.6/examples/__init__.py` & `bw_temporalis-0.7/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.6/examples/ia.py` & `bw_temporalis-0.7/examples/ia.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.6/examples/inv.py` & `bw_temporalis-0.7/examples/inv.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.6/setup.cfg` & `bw_temporalis-0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.6/tests/test_convolution.py` & `bw_temporalis-0.7/tests/test_convolution.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.6/tests/test_fixtures.py` & `bw_temporalis-0.7/tests/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.6/tests/test_lca.py` & `bw_temporalis-0.7/tests/test_lca.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.6/tests/test_td.py` & `bw_temporalis-0.7/tests/test_td.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,26 +162,26 @@
 
 def test_repr(simple):
     assert repr(simple)
 
 
 def test_simplify_timedelta():
     td = easy_timedelta_distribution(
-        start=0, end=500, steps=250, resolution="D"
+        start=0, end=500, steps=1500, resolution="D"
     ).simplify()
     assert td.date.dtype == np.dtype("timedelta64[s]")
     assert np.allclose(td.amount.sum(), 1)
-    assert len(td) <= 100
+    assert len(td) <= 1000
     assert td.date.min() >= np.array(0, dtype="timedelta64[D]")
     assert td.date.max() <= np.array(500, dtype="timedelta64[D]")
 
 
 def test_simplify_timedelta_num_clusters():
     td = easy_timedelta_distribution(
-        start=0, end=500, steps=250, resolution="D"
+        start=0, end=500, steps=1250, resolution="D"
     ).simplify(num_clusters=25)
     assert td.date.dtype == np.dtype("timedelta64[s]")
     assert np.allclose(td.amount.sum(), 1)
     assert len(td) <= 25
     assert td.date.min() >= np.array(0, dtype="timedelta64[D]")
     assert td.date.max() <= np.array(500, dtype="timedelta64[D]")
 
@@ -191,14 +191,14 @@
         start=0, end=500, steps=25, resolution="D"
     ).simplify()
     assert td.simplify() is td
 
 
 def test_simplify_datetime():
     td = easy_datetime_distribution(
-        start="2023-01-01", end="2023-12-31", steps=250
+        start="2023-01-01", end="2023-12-31", steps=1500
     ).simplify()
     assert td.date.dtype == np.dtype("datetime64[s]")
     assert np.allclose(td.amount.sum(), 1)
-    assert len(td) <= 100
+    assert len(td) <= 1000
     assert td.date.min() >= np.array("2023-01-01", dtype="datetime64[s]")
     assert td.date.max() <= np.array("2023-12-31", dtype="datetime64[s]")
```

### Comparing `bw_temporalis-0.6/tests/test_timeline.py` & `bw_temporalis-0.7/tests/test_timeline.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.6/tests/test_utils.py` & `bw_temporalis-0.7/tests/test_utils.py`

 * *Files identical despite different names*

