# Comparing `tmp/meow-sim-0.5.1.tar.gz` & `tmp/meow-sim-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meow-sim-0.5.1.tar", last modified: Wed Jun  7 14:51:36 2023, max compression
+gzip compressed data, was "meow-sim-0.5.2.tar", last modified: Thu Jun  8 00:26:58 2023, max compression
```

## Comparing `meow-sim-0.5.1.tar` & `meow-sim-0.5.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 14:51:36.654299 meow-sim-0.5.1/
--rw-r--r--   0 root         (0) root         (0)    11347 2023-06-07 14:51:31.000000 meow-sim-0.5.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3078 2023-06-07 14:51:36.650298 meow-sim-0.5.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2060 2023-06-07 14:51:31.000000 meow-sim-0.5.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 14:51:36.650298 meow-sim-0.5.1/meow/
--rw-r--r--   0 root         (0) root         (0)     1414 2023-06-07 14:51:31.000000 meow-sim-0.5.1/meow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 14:51:36.650298 meow-sim-0.5.1/meow/assets/
--rw-r--r--   0 root         (0) root         (0)    10307 2023-06-07 14:51:31.000000 meow-sim-0.5.1/meow/assets/silicon.csv
--rw-r--r--   0 root         (0) root         (0)     8535 2023-06-07 14:51:31.000000 meow-sim-0.5.1/meow/assets/silicon_oxide.csv
--rw-r--r--   0 root         (0) root         (0)     8019 2023-06-07 14:51:31.000000 meow-sim-0.5.1/meow/base_model.py
--rw-r--r--   0 root         (0) root         (0)     1189 2023-06-07 14:51:31.000000 meow-sim-0.5.1/meow/cache.py
--rw-r--r--   0 root         (0) root         (0)     4844 2023-06-07 14:51:31.000000 meow-sim-0.5.1/meow/cell.py
--rw-r--r--   0 root         (0) root         (0)     2797 2023-06-07 14:51:31.000000 meow-sim-0.5.1/meow/cross_section.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 14:51:36.650298 meow-sim-0.5.1/meow/eme/
--rw-r--r--   0 root         (0) root         (0)      623 2023-06-07 14:51:31.000000 meow-sim-0.5.1/meow/eme/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5533 2023-06-07 14:51:31.000000 meow-sim-0.5.1/meow/eme/common.py
--rw-r--r--   0 root         (0) root         (0)     3810 2023-06-07 14:51:31.000000 meow-sim-0.5.1/meow/eme/sax.py
--rw-r--r--   0 root         (0) root         (0)      551 2023-06-07 14:51:31.000000 meow-sim-0.5.1/meow/environment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 14:51:36.650298 meow-sim-0.5.1/meow/fde/
--rw-r--r--   0 root         (0) root         (0)      324 2023-06-07 14:51:31.000000 meow-sim-0.5.1/meow/fde/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4621 2023-06-07 14:51:31.000000 meow-sim-0.5.1/meow/fde/lumerical.py
--rw-r--r--   0 root         (0) root         (0)     2969 2023-06-07 14:51:31.000000 meow-sim-0.5.1/meow/fde/tidy3d.py
--rw-r--r--   0 root         (0) root         (0)     2318 2023-06-07 14:51:31.000000 meow-sim-0.5.1/meow/gds_structures.py
--rw-r--r--   0 root         (0) root         (0)    10642 2023-06-07 14:51:31.000000 meow-sim-0.5.1/meow/geometries.py
--rw-r--r--   0 root         (0) root         (0)      960 2023-06-07 14:51:31.000000 meow-sim-0.5.1/meow/integrate.py
--rw-r--r--   0 root         (0) root         (0)    10798 2023-06-07 14:51:31.000000 meow-sim-0.5.1/meow/materials.py
--rw-r--r--   0 root         (0) root         (0)     3579 2023-06-07 14:51:31.000000 meow-sim-0.5.1/meow/mesh.py
--rw-r--r--   0 root         (0) root         (0)    12861 2023-06-07 14:51:31.000000 meow-sim-0.5.1/meow/mode.py
--rw-r--r--   0 root         (0) root         (0)     1876 2023-06-07 14:51:31.000000 meow-sim-0.5.1/meow/structures.py
--rw-r--r--   0 root         (0) root         (0)     7658 2023-06-07 14:51:31.000000 meow-sim-0.5.1/meow/visualize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 14:51:36.650298 meow-sim-0.5.1/meow_sim.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3078 2023-06-07 14:51:36.000000 meow-sim-0.5.1/meow_sim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      686 2023-06-07 14:51:36.000000 meow-sim-0.5.1/meow_sim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 14:51:36.000000 meow-sim-0.5.1/meow_sim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      408 2023-06-07 14:51:36.000000 meow-sim-0.5.1/meow_sim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-07 14:51:36.000000 meow-sim-0.5.1/meow_sim.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1819 2023-06-07 14:51:31.000000 meow-sim-0.5.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-07 14:51:36.654299 meow-sim-0.5.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 14:51:36.650298 meow-sim-0.5.1/tests/
--rw-r--r--   0 root         (0) root         (0)     3931 2023-06-07 14:51:31.000000 meow-sim-0.5.1/tests/test_deserialization.py
--rw-r--r--   0 root         (0) root         (0)     3767 2023-06-07 14:51:31.000000 meow-sim-0.5.1/tests/test_mode_operators.py
--rw-r--r--   0 root         (0) root         (0)     1322 2023-06-07 14:51:31.000000 meow-sim-0.5.1/tests/test_nbs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:26:58.972550 meow-sim-0.5.2/
+-rw-r--r--   0 root         (0) root         (0)    11347 2023-06-08 00:26:54.000000 meow-sim-0.5.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-06-08 00:26:58.972550 meow-sim-0.5.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2223 2023-06-08 00:26:54.000000 meow-sim-0.5.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:26:58.972550 meow-sim-0.5.2/meow/
+-rw-r--r--   0 root         (0) root         (0)     1414 2023-06-08 00:26:54.000000 meow-sim-0.5.2/meow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:26:58.972550 meow-sim-0.5.2/meow/assets/
+-rw-r--r--   0 root         (0) root         (0)    10307 2023-06-08 00:26:54.000000 meow-sim-0.5.2/meow/assets/silicon.csv
+-rw-r--r--   0 root         (0) root         (0)     8535 2023-06-08 00:26:54.000000 meow-sim-0.5.2/meow/assets/silicon_oxide.csv
+-rw-r--r--   0 root         (0) root         (0)     8019 2023-06-08 00:26:54.000000 meow-sim-0.5.2/meow/base_model.py
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-06-08 00:26:54.000000 meow-sim-0.5.2/meow/cache.py
+-rw-r--r--   0 root         (0) root         (0)     4844 2023-06-08 00:26:54.000000 meow-sim-0.5.2/meow/cell.py
+-rw-r--r--   0 root         (0) root         (0)     2797 2023-06-08 00:26:54.000000 meow-sim-0.5.2/meow/cross_section.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:26:58.972550 meow-sim-0.5.2/meow/eme/
+-rw-r--r--   0 root         (0) root         (0)      623 2023-06-08 00:26:54.000000 meow-sim-0.5.2/meow/eme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5533 2023-06-08 00:26:54.000000 meow-sim-0.5.2/meow/eme/common.py
+-rw-r--r--   0 root         (0) root         (0)     3810 2023-06-08 00:26:54.000000 meow-sim-0.5.2/meow/eme/sax.py
+-rw-r--r--   0 root         (0) root         (0)      551 2023-06-08 00:26:54.000000 meow-sim-0.5.2/meow/environment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:26:58.972550 meow-sim-0.5.2/meow/fde/
+-rw-r--r--   0 root         (0) root         (0)      324 2023-06-08 00:26:54.000000 meow-sim-0.5.2/meow/fde/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4621 2023-06-08 00:26:54.000000 meow-sim-0.5.2/meow/fde/lumerical.py
+-rw-r--r--   0 root         (0) root         (0)     2969 2023-06-08 00:26:54.000000 meow-sim-0.5.2/meow/fde/tidy3d.py
+-rw-r--r--   0 root         (0) root         (0)     2318 2023-06-08 00:26:54.000000 meow-sim-0.5.2/meow/gds_structures.py
+-rw-r--r--   0 root         (0) root         (0)    10642 2023-06-08 00:26:54.000000 meow-sim-0.5.2/meow/geometries.py
+-rw-r--r--   0 root         (0) root         (0)      960 2023-06-08 00:26:54.000000 meow-sim-0.5.2/meow/integrate.py
+-rw-r--r--   0 root         (0) root         (0)    10798 2023-06-08 00:26:54.000000 meow-sim-0.5.2/meow/materials.py
+-rw-r--r--   0 root         (0) root         (0)     3579 2023-06-08 00:26:54.000000 meow-sim-0.5.2/meow/mesh.py
+-rw-r--r--   0 root         (0) root         (0)    12966 2023-06-08 00:26:54.000000 meow-sim-0.5.2/meow/mode.py
+-rw-r--r--   0 root         (0) root         (0)     1876 2023-06-08 00:26:54.000000 meow-sim-0.5.2/meow/structures.py
+-rw-r--r--   0 root         (0) root         (0)     7469 2023-06-08 00:26:54.000000 meow-sim-0.5.2/meow/visualize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:26:58.972550 meow-sim-0.5.2/meow_sim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-06-08 00:26:58.000000 meow-sim-0.5.2/meow_sim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      686 2023-06-08 00:26:58.000000 meow-sim-0.5.2/meow_sim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 00:26:58.000000 meow-sim-0.5.2/meow_sim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      408 2023-06-08 00:26:58.000000 meow-sim-0.5.2/meow_sim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-08 00:26:58.000000 meow-sim-0.5.2/meow_sim.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1819 2023-06-08 00:26:54.000000 meow-sim-0.5.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 00:26:58.972550 meow-sim-0.5.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:26:58.972550 meow-sim-0.5.2/tests/
+-rw-r--r--   0 root         (0) root         (0)     3931 2023-06-08 00:26:54.000000 meow-sim-0.5.2/tests/test_deserialization.py
+-rw-r--r--   0 root         (0) root         (0)     3767 2023-06-08 00:26:54.000000 meow-sim-0.5.2/tests/test_mode_operators.py
+-rw-r--r--   0 root         (0) root         (0)     1322 2023-06-08 00:26:54.000000 meow-sim-0.5.2/tests/test_nbs.py
```

### Comparing `meow-sim-0.5.1/LICENSE` & `meow-sim-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.1/PKG-INFO` & `meow-sim-0.5.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.5.1
+Version: 0.5.2
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -66,14 +66,19 @@
 
 
 ## Documentation
 
 - [Examples](https://flaport.github.io/meow/examples.html)
 - [API Docs](https://flaport.github.io/meow/meow.html)
 
+## Contributors
+
+- [@flaport](https://gitub.com/flaport): creator of MEOW
+- [@jan-david-black](https://github.com/jan-david-black): fixing mode overlaps and more
+
 ## Credits
 
 - [DALL-E](https://labs.openai.com): _“a drawing of a kitten with laser eyes walking towards me”_ (logo)
 - [Tidy3D](https://github.com/flexcompute/tidy3d): meow uses the free FDE mode solver from Tidy3D.
 - [SAX](https://github.com/flaport/sax): meow uses SAX as its circuit simulator when cascading the overlap S-matrices.
 - [klujax](https://github.com/flaport/sax): Although technically an optional backend for SAX, klujax will significantly speed up the final S-matrix calculation of your structures.
 - [EMEPy](https://github.com/BYUCamachoLab/emepy): an excellent alternative python-based EME solver with optional neural network mode solver.
```

### Comparing `meow-sim-0.5.1/README.md` & `meow-sim-0.5.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -37,14 +37,19 @@
 
 
 ## Documentation
 
 - [Examples](https://flaport.github.io/meow/examples.html)
 - [API Docs](https://flaport.github.io/meow/meow.html)
 
+## Contributors
+
+- [@flaport](https://gitub.com/flaport): creator of MEOW
+- [@jan-david-black](https://github.com/jan-david-black): fixing mode overlaps and more
+
 ## Credits
 
 - [DALL-E](https://labs.openai.com): _“a drawing of a kitten with laser eyes walking towards me”_ (logo)
 - [Tidy3D](https://github.com/flexcompute/tidy3d): meow uses the free FDE mode solver from Tidy3D.
 - [SAX](https://github.com/flaport/sax): meow uses SAX as its circuit simulator when cascading the overlap S-matrices.
 - [klujax](https://github.com/flaport/sax): Although technically an optional backend for SAX, klujax will significantly speed up the final S-matrix calculation of your structures.
 - [EMEPy](https://github.com/BYUCamachoLab/emepy): an excellent alternative python-based EME solver with optional neural network mode solver.
```

### Comparing `meow-sim-0.5.1/meow/__init__.py` & `meow-sim-0.5.2/meow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ MEOW: Modeling of Eigenmodes and Overlaps in Waveguides """
 
 __author__ = "Floris Laporte"
-__version__ = "0.5.1"
+__version__ = "0.5.2"
 
 import warnings
 
 # Silence Excessive Logging...
 
 try:
     from loguru import logger
```

### Comparing `meow-sim-0.5.1/meow/assets/silicon.csv` & `meow-sim-0.5.2/meow/assets/silicon.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.1/meow/assets/silicon_oxide.csv` & `meow-sim-0.5.2/meow/assets/silicon_oxide.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.1/meow/base_model.py` & `meow-sim-0.5.2/meow/base_model.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.1/meow/cache.py` & `meow-sim-0.5.2/meow/cache.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.1/meow/cell.py` & `meow-sim-0.5.2/meow/cell.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.1/meow/cross_section.py` & `meow-sim-0.5.2/meow/cross_section.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.1/meow/eme/__init__.py` & `meow-sim-0.5.2/meow/eme/__init__.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.1/meow/eme/common.py` & `meow-sim-0.5.2/meow/eme/common.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.1/meow/eme/sax.py` & `meow-sim-0.5.2/meow/eme/sax.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.1/meow/environment.py` & `meow-sim-0.5.2/meow/environment.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.1/meow/fde/lumerical.py` & `meow-sim-0.5.2/meow/fde/lumerical.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.1/meow/fde/tidy3d.py` & `meow-sim-0.5.2/meow/fde/tidy3d.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.1/meow/gds_structures.py` & `meow-sim-0.5.2/meow/gds_structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.1/meow/geometries.py` & `meow-sim-0.5.2/meow/geometries.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.1/meow/integrate.py` & `meow-sim-0.5.2/meow/integrate.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.1/meow/materials.py` & `meow-sim-0.5.2/meow/materials.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.1/meow/mesh.py` & `meow-sim-0.5.2/meow/mesh.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.1/meow/mode.py` & `meow-sim-0.5.2/meow/mode.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,14 +111,15 @@
     @property
     def cell(self):
         return self.cs.cell
 
     def _visualize(
         self,
         title=None,
+        title_prefix="",
         fields=None,
         ax=None,
         n_cmap=None,
         mode_cmap=None,
         num_levels=8,
         operation=lambda x: np.abs(x) ** 2,
         show=True,
@@ -142,14 +143,15 @@
                 raise ValueError(
                     f"Not enough axes supplied for the number of fields "
                     f"to plot! {len(ax)} < {len(fields)}."
                 )
             for field, ax_ in zip(fields, ax):
                 self._visualize(
                     title=title,
+                    title_prefix=title_prefix,
                     fields=[field],
                     ax=ax_,
                     n_cmap=n_cmap,
                     mode_cmap=mode_cmap,
                     num_levels=num_levels,
                     operation=operation,
                     show=False,
@@ -191,17 +193,17 @@
 
         n = np.real(getattr(self.cs, f"n{c}"))
         plt.pcolormesh(X, Y, n, cmap=n_cmap)
         plt.xlabel(x)
         plt.ylabel(y)
         plt.grid(True, alpha=0.4)
         if title is None:
-            plt.title(f"{field} [neff={float(np.real(self.neff)):.6f}]")
+            plt.title(f"{title_prefix}{field} [neff={float(np.real(self.neff)):.6f}]")
         else:
-            plt.title(title)
+            plt.title(f"{title_prefix}{title}")
         plt.xlim(X.min(), X.max())
         plt.ylim(Y.min(), Y.max())
         plt.axis("scaled")
         if show:
             plt.show()
 
     def save(self, filename):
```

### Comparing `meow-sim-0.5.1/meow/structures.py` & `meow-sim-0.5.2/meow/structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.1/meow/visualize.py` & `meow-sim-0.5.2/meow/visualize.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,19 +70,19 @@
     if title is not None:
         plt.title(title)
 
     if show:
         plt.show()
 
 
-def _visualize_s_pm_matrix(Spm, fmt=None, title=None, show=True, ax=None):
+def _visualize_s_pm_matrix(Spm, fmt=None, title=None, show=True, phase=False, ax=None):
     import matplotlib.pyplot as plt  # fmt: skip
 
     S, pm = Spm
-    _visualize_s_matrix(S, fmt=fmt, title=title, show=False, ax=ax)
+    _visualize_s_matrix(S, fmt=fmt, title=title, show=False, phase=phase, ax=ax)
     num_left = len([p for p in pm if "left" in p])
     Z = np.abs(S)
     _, x = np.arange(Z.shape[0])[::-1], np.arange(Z.shape[1])
 
     plt.axvline(x[num_left] - 0.5, color="red")
     plt.axhline(x[num_left] - 0.5, color="red")
 
@@ -210,36 +210,32 @@
     n_cmap=None,
     mode_cmap=None,
     num_levels=8,
     operation=lambda x: np.abs(x) ** 2,
     show=True,
 ):
     import matplotlib.pyplot as plt  # fmt: skip
-    from matplotlib.colors import LinearSegmentedColormap  # fmt: skip
-    from mpl_toolkits.axes_grid1 import make_axes_locatable  # fmt: skip
 
     num_modes = len(modes)
     cs = modes[0].cs
     X, Y, n = cs.mesh.Xz, cs.mesh.Yz, cs.nz
     W, H = _figsize_visualize_mode(cs, 6.4)
 
-    n_cmap = LinearSegmentedColormap.from_list(
-        name="c_cmap", colors=["#ffffff", "#c1d9ed"]
-    )
     fig, ax = plt.subplots(
         num_modes,
         2,
         figsize=(2 * W, num_modes * H),
         sharex=True,
         sharey=True,
         squeeze=False,
     )
     for i, m in enumerate(modes):
         m._visualize(
             title=None,
+            title_prefix=f"m{i}: ",
             fields=["Ex", "Hx"],
             ax=ax[i],
             n_cmap=n_cmap,
             mode_cmap=mode_cmap,
             num_levels=num_levels,
             operation=operation,
             show=False,
```

### Comparing `meow-sim-0.5.1/meow_sim.egg-info/PKG-INFO` & `meow-sim-0.5.2/meow_sim.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.5.1
+Version: 0.5.2
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -66,14 +66,19 @@
 
 
 ## Documentation
 
 - [Examples](https://flaport.github.io/meow/examples.html)
 - [API Docs](https://flaport.github.io/meow/meow.html)
 
+## Contributors
+
+- [@flaport](https://gitub.com/flaport): creator of MEOW
+- [@jan-david-black](https://github.com/jan-david-black): fixing mode overlaps and more
+
 ## Credits
 
 - [DALL-E](https://labs.openai.com): _“a drawing of a kitten with laser eyes walking towards me”_ (logo)
 - [Tidy3D](https://github.com/flexcompute/tidy3d): meow uses the free FDE mode solver from Tidy3D.
 - [SAX](https://github.com/flaport/sax): meow uses SAX as its circuit simulator when cascading the overlap S-matrices.
 - [klujax](https://github.com/flaport/sax): Although technically an optional backend for SAX, klujax will significantly speed up the final S-matrix calculation of your structures.
 - [EMEPy](https://github.com/BYUCamachoLab/emepy): an excellent alternative python-based EME solver with optional neural network mode solver.
```

### Comparing `meow-sim-0.5.1/meow_sim.egg-info/SOURCES.txt` & `meow-sim-0.5.2/meow_sim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.1/pyproject.toml` & `meow-sim-0.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["build", "pip", "setuptools", "wheel", "pybind11"]
 
 [project]
 name = "meow-sim"
-version = "0.5.1"
+version = "0.5.2"
 authors = [
 { name = "Rockley Photonics" },
 { name = "Floris Laporte", email = "floris.laporte@rockleyphotonics.com" },
 ]
 description = "Modeling of Eigenmodes and Overlaps in Waveguide Structures"
 requires-python = ">=3.8"
 keywords = [
```

### Comparing `meow-sim-0.5.1/tests/test_deserialization.py` & `meow-sim-0.5.2/tests/test_deserialization.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.1/tests/test_mode_operators.py` & `meow-sim-0.5.2/tests/test_mode_operators.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.1/tests/test_nbs.py` & `meow-sim-0.5.2/tests/test_nbs.py`

 * *Files identical despite different names*

