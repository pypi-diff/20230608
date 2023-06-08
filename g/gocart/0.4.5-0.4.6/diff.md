# Comparing `tmp/gocart-0.4.5.tar.gz` & `tmp/gocart-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gocart-0.4.5.tar", last modified: Tue Jun  6 15:31:31 2023, max compression
+gzip compressed data, was "gocart-0.4.6.tar", last modified: Thu Jun  8 15:34:23 2023, max compression
```

## Comparing `gocart-0.4.5.tar` & `gocart-0.4.6.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-06 15:31:31.127103 gocart-0.4.5/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     4516 2023-06-06 15:25:02.000000 gocart-0.4.5/CHANGES.md
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    35149 2023-06-06 15:25:02.000000 gocart-0.4.5/LICENSE
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      377 2023-06-06 15:25:02.000000 gocart-0.4.5/MANIFEST.in
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6460 2023-06-06 15:31:31.127103 gocart-0.4.5/PKG-INFO
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5894 2023-06-06 15:25:02.000000 gocart-0.4.5/README.md
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-06 15:31:31.107102 gocart-0.4.5/gocart/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      189 2023-06-06 15:25:02.000000 gocart-0.4.5/gocart/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       22 2023-06-06 15:25:02.000000 gocart-0.4.5/gocart/__version__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      738 2023-06-06 15:25:02.000000 gocart-0.4.5/gocart/advanced_settings.yaml
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    10717 2023-06-06 15:25:02.000000 gocart-0.4.5/gocart/cl_utils.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-06 15:31:31.115102 gocart-0.4.5/gocart/commonutils/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      157 2023-06-06 15:25:02.000000 gocart-0.4.5/gocart/commonutils/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     4510 2023-06-06 15:25:02.000000 gocart-0.4.5/gocart/commonutils/flatten_healpix_map.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3054 2023-06-06 15:25:02.000000 gocart-0.4.5/gocart/commonutils/generate_skymap_stats.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      358 2023-06-06 15:25:02.000000 gocart-0.4.5/gocart/commonutils/getpackagepath.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-06 15:31:31.123103 gocart-0.4.5/gocart/convert/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      204 2023-06-06 15:25:02.000000 gocart-0.4.5/gocart/convert/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    14318 2023-06-06 15:25:02.000000 gocart-0.4.5/gocart/convert/aitoff.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3397 2023-06-06 15:25:02.000000 gocart-0.4.5/gocart/convert/ascii.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6489 2023-06-06 15:25:02.000000 gocart-0.4.5/gocart/convert/healpix2cart.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3096 2023-06-06 15:25:02.000000 gocart-0.4.5/gocart/default_settings.yaml
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-06 15:31:31.123103 gocart-0.4.5/gocart/parsers/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       56 2023-06-06 15:25:02.000000 gocart-0.4.5/gocart/parsers/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    16347 2023-06-06 15:25:02.000000 gocart-0.4.5/gocart/parsers/lvk.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-06 15:31:31.095102 gocart-0.4.5/gocart/resources/
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-06 15:31:31.127103 gocart-0.4.5/gocart/resources/plugins/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3124 2023-06-06 15:25:03.000000 gocart-0.4.5/gocart/resources/plugins/gp_template.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     9654 2023-06-06 15:25:03.000000 gocart-0.4.5/gocart/setup.cfg
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2891 2023-06-06 15:25:03.000000 gocart-0.4.5/gocart/test_settings.yaml
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3387 2023-06-06 15:25:03.000000 gocart-0.4.5/gocart/utKit.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-06 15:31:31.111102 gocart-0.4.5/gocart.egg-info/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6460 2023-06-06 15:31:30.000000 gocart-0.4.5/gocart.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      788 2023-06-06 15:31:30.000000 gocart-0.4.5/gocart.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-06-06 15:31:30.000000 gocart-0.4.5/gocart.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       48 2023-06-06 15:31:30.000000 gocart-0.4.5/gocart.egg-info/entry_points.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-06-06 15:29:38.000000 gocart-0.4.5/gocart.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      109 2023-06-06 15:31:30.000000 gocart-0.4.5/gocart.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        7 2023-06-06 15:31:30.000000 gocart-0.4.5/gocart.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       38 2023-06-06 15:31:31.127103 gocart-0.4.5/setup.cfg
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1915 2023-06-06 15:25:03.000000 gocart-0.4.5/setup.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-08 15:34:23.523552 gocart-0.4.6/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     4711 2023-06-08 15:28:52.000000 gocart-0.4.6/CHANGES.md
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    35149 2023-06-08 15:28:52.000000 gocart-0.4.6/LICENSE
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      377 2023-06-08 15:28:52.000000 gocart-0.4.6/MANIFEST.in
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6460 2023-06-08 15:34:23.523552 gocart-0.4.6/PKG-INFO
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5894 2023-06-08 15:28:52.000000 gocart-0.4.6/README.md
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-08 15:34:23.499551 gocart-0.4.6/gocart/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      189 2023-06-08 15:28:52.000000 gocart-0.4.6/gocart/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       22 2023-06-08 15:28:52.000000 gocart-0.4.6/gocart/__version__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      738 2023-06-08 15:28:52.000000 gocart-0.4.6/gocart/advanced_settings.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    10717 2023-06-08 15:28:52.000000 gocart-0.4.6/gocart/cl_utils.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-08 15:34:23.515551 gocart-0.4.6/gocart/commonutils/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      200 2023-06-08 15:28:52.000000 gocart-0.4.6/gocart/commonutils/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     4510 2023-06-08 15:28:52.000000 gocart-0.4.6/gocart/commonutils/flatten_healpix_map.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3054 2023-06-08 15:28:52.000000 gocart-0.4.6/gocart/commonutils/generate_skymap_stats.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      358 2023-06-08 15:28:52.000000 gocart-0.4.6/gocart/commonutils/getpackagepath.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-08 15:34:23.515551 gocart-0.4.6/gocart/convert/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      204 2023-06-08 15:28:52.000000 gocart-0.4.6/gocart/convert/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    14497 2023-06-08 15:28:52.000000 gocart-0.4.6/gocart/convert/aitoff.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3397 2023-06-08 15:28:52.000000 gocart-0.4.6/gocart/convert/ascii.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6489 2023-06-08 15:28:52.000000 gocart-0.4.6/gocart/convert/healpix2cart.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3096 2023-06-08 15:28:52.000000 gocart-0.4.6/gocart/default_settings.yaml
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-08 15:34:23.519552 gocart-0.4.6/gocart/parsers/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       56 2023-06-08 15:28:52.000000 gocart-0.4.6/gocart/parsers/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    16347 2023-06-08 15:28:52.000000 gocart-0.4.6/gocart/parsers/lvk.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-08 15:34:23.519552 gocart-0.4.6/gocart/resources/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6885 2023-06-08 15:28:52.000000 gocart-0.4.6/gocart/resources/package.mplstyle
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-08 15:34:23.519552 gocart-0.4.6/gocart/resources/plugins/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3124 2023-06-08 15:28:52.000000 gocart-0.4.6/gocart/resources/plugins/gp_template.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     9654 2023-06-08 15:28:52.000000 gocart-0.4.6/gocart/setup.cfg
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2891 2023-06-08 15:28:52.000000 gocart-0.4.6/gocart/test_settings.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3387 2023-06-08 15:28:52.000000 gocart-0.4.6/gocart/utKit.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-08 15:34:23.507551 gocart-0.4.6/gocart.egg-info/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6460 2023-06-08 15:34:23.000000 gocart-0.4.6/gocart.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      822 2023-06-08 15:34:23.000000 gocart-0.4.6/gocart.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-06-08 15:34:23.000000 gocart-0.4.6/gocart.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       48 2023-06-08 15:34:23.000000 gocart-0.4.6/gocart.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-06-08 15:32:49.000000 gocart-0.4.6/gocart.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      109 2023-06-08 15:34:23.000000 gocart-0.4.6/gocart.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        7 2023-06-08 15:34:23.000000 gocart-0.4.6/gocart.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       38 2023-06-08 15:34:23.523552 gocart-0.4.6/setup.cfg
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1915 2023-06-08 15:28:52.000000 gocart-0.4.6/setup.py
```

### Comparing `gocart-0.4.5/CHANGES.md` & `gocart-0.4.6/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 
 ## Release Notes
 
+**v0.4.6 - June 8, 2023**
+
+- **REFACTOR**: making plots consistent across platforms by including a MPL style file
+- **FIXED**: area of contours now included in plots if generated from a plugin
+
 **v0.4.5 - June 6, 2023**
 
 - **FEATURE**: added ability to plot square footprints on to the aitoff skymaps  
 - **ENHANCEMENT**: significance explicitly added to RHS sidebar of maps  
 - **REFACTOR**: colours of map contours adjusted to pastel colours  
 - **REFACTOR**: transparency of sun, moon, galactic plane adjusted for greater clarity  
 - **FIXED**: contours often getting tangled at the poles of the aitoff maps and rendering incorrectly. Solved by 'chunking' the filled contours with matplotlib  
@@ -34,15 +39,15 @@
 - **ENHANCEMENT**: redshift range added to the right side of aitoff plots  
 - **REFACTOR**: removed `ligo.skymap` dependency as this is a huge package and was causing upgrades of gocart to take 20-40 mins. Required new code to convert multi-order skymaps to a single-order (I was previously relying on a function in `ligo.skymap` to do this)  
 
 **v0.3.0 - May 18, 2023**  
 
 - **FEATURE**: user can now add their own plugin scripts to run every time an alert is parsed  
 - **ENHANCEMENT**: added a count of alerts read when first connected to kafka (gives users peace of mind that goacrt is working)  
-- **FIXED**: area calulations fixed (I was still sort by prob but should have been sorting by probdensity for mulit-order maps)  
+- **FIXED**: area calculations fixed (I was still sort by prob but should have been sorting by probdensity for mulit-order maps)  
 - **FIXED**: can still read an event ID even if not found in the sky-map header (tried to find the event ID from the map directory path)  
 
 **v0.2.1 - April 26, 2023**  
 
 - **FIXED**: listen command was tripping up on mock-events
 
 **v0.2.0 - April 26, 2023**
```

### Comparing `gocart-0.4.5/LICENSE` & `gocart-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gocart-0.4.5/PKG-INFO` & `gocart-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: gocart
-Version: 0.4.5
+Version: 0.4.6
 Summary: Listen for, collect and convert multimessenger skymaps
 Home-page: https://github.com/thespacedoctor/gocart
-Download-URL: https://github.com/thespacedoctor/gocart/archive/v0.4.5.zip
+Download-URL: https://github.com/thespacedoctor/gocart/archive/v0.4.6.zip
 Author: David Young
 Author-email: d.r.young@qub.ac.uk
 License: MIT
 Keywords: astronomy
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `gocart-0.4.5/README.md` & `gocart-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `gocart-0.4.5/gocart/advanced_settings.yaml` & `gocart-0.4.6/gocart/advanced_settings.yaml`

 * *Files identical despite different names*

### Comparing `gocart-0.4.5/gocart/cl_utils.py` & `gocart-0.4.6/gocart/cl_utils.py`

 * *Files identical despite different names*

### Comparing `gocart-0.4.5/gocart/commonutils/flatten_healpix_map.py` & `gocart-0.4.6/gocart/commonutils/flatten_healpix_map.py`

 * *Files identical despite different names*

### Comparing `gocart-0.4.5/gocart/commonutils/generate_skymap_stats.py` & `gocart-0.4.6/gocart/commonutils/generate_skymap_stats.py`

 * *Files identical despite different names*

### Comparing `gocart-0.4.5/gocart/convert/aitoff.py` & `gocart-0.4.6/gocart/convert/aitoff.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,27 +92,32 @@
 
         **Return:**
             - ``plotPath`` -- path to the printed plot
         """
         self.log.debug('starting the ``convert`` method')
 
         import matplotlib.pyplot as plt
+        from gocart.commonutils import getpackagepath
+        styleFile = getpackagepath() + "/resources/package.mplstyle"
+        plt.style.use(styleFile)
+
         from . import healpix2cart
         import astropy.units as u
         import numpy as np
         from astropy.coordinates import SkyCoord, Galactic, get_sun, get_body
         from matplotlib.projections.geo import GeoAxes
         from matplotlib.cm import get_cmap
         import matplotlib.patches as mpatches
         from matplotlib.lines import Line2D
         from astropy.time import Time
         from matplotlib.collections import PatchCollection
 
         import matplotlib
-        # matplotlib.use('PDF')
+
+        matplotlib.use('PDF')
         # plt.ion()
 
         class ThetaFormatterShiftPi(GeoAxes.ThetaFormatter):
             """SHIFTS LABELLING BY PI
             SHIFTS LABELLING FROM -180,180 TO 360-0"""
 
             def __call__(self, x, pos=None):
@@ -278,19 +283,19 @@
 
             z = 10
 
             for c, l in zip(colors, levels):
                 z += 1
                 ax.contourf(long, lat,
                             contours, levels=[-1, l], colors=c, zorder=z, alpha=1., nchunk=10, antialiased=False)
-                if "EXTRA" in self.meta and f"area{l}" in self.meta["EXTRA"]:
-                    area = self.meta["EXTRA"][f"area{l}"]
-                    label = f"{l}%: {area:.1f} deg$^2$"
+                if "EXTRA" in self.meta and f"area{int(l)}" in self.meta["EXTRA"]:
+                    area = self.meta["EXTRA"][f"area{int(l)}"]
+                    label = f"{int(l)}%: {area:.1f} deg$^2$"
                 else:
-                    label = f"{l}%"
+                    label = f"{int(l)}%"
                 patch = mpatches.Patch(color=c, label=label)
                 handles.append(patch)
 
         if len(self.meta):
             data = ""
             data += f"Event: {self.meta['ALERT']['superevent_id']} ({self.meta['ALERT']['event']['group']})\n"
             eventDate = Time(self.meta['HEADER']['DATE-OBS'], scale='utc').to_datetime().strftime("%Y-%m-%d %H:%M:%S")
@@ -346,15 +351,15 @@
             if self.patchesLabel:
                 patch = mpatches.Patch(color=self.patchesColor, label=self.patchesLabel)
                 handles.append(patch)
 
         ax.tick_params(axis='x', labelsize=12)
         ax.tick_params(axis='y', labelsize=12)
         ax.grid(color='#657b83', alpha=0.4, linestyle='dotted')
-        plt.legend(handles=handles, loc='upper left', scatterpoints=1, bbox_to_anchor=(1.01, 1), fontsize=6)
+        plt.legend(handles=handles, loc='upper left', scatterpoints=1, bbox_to_anchor=(1.01, 1.02), fontsize=6)
         ax.xaxis.zorder = 40
         ax.yaxis.zorder = 40
 
         plt.grid(True)
 
         plt.savefig(self.outputFolder + f"/{self.plotName}", bbox_inches='tight', dpi=300)
```

### Comparing `gocart-0.4.5/gocart/convert/ascii.py` & `gocart-0.4.6/gocart/convert/ascii.py`

 * *Files identical despite different names*

### Comparing `gocart-0.4.5/gocart/convert/healpix2cart.py` & `gocart-0.4.6/gocart/convert/healpix2cart.py`

 * *Files identical despite different names*

### Comparing `gocart-0.4.5/gocart/default_settings.yaml` & `gocart-0.4.6/gocart/default_settings.yaml`

 * *Files identical despite different names*

### Comparing `gocart-0.4.5/gocart/parsers/lvk.py` & `gocart-0.4.6/gocart/parsers/lvk.py`

 * *Files identical despite different names*

### Comparing `gocart-0.4.5/gocart/resources/plugins/gp_template.py` & `gocart-0.4.6/gocart/resources/plugins/gp_template.py`

 * *Files identical despite different names*

### Comparing `gocart-0.4.5/gocart/setup.cfg` & `gocart-0.4.6/gocart/setup.cfg`

 * *Files identical despite different names*

### Comparing `gocart-0.4.5/gocart/test_settings.yaml` & `gocart-0.4.6/gocart/test_settings.yaml`

 * *Files identical despite different names*

### Comparing `gocart-0.4.5/gocart/utKit.py` & `gocart-0.4.6/gocart/utKit.py`

 * *Files identical despite different names*

### Comparing `gocart-0.4.5/gocart.egg-info/PKG-INFO` & `gocart-0.4.6/gocart.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: gocart
-Version: 0.4.5
+Version: 0.4.6
 Summary: Listen for, collect and convert multimessenger skymaps
 Home-page: https://github.com/thespacedoctor/gocart
-Download-URL: https://github.com/thespacedoctor/gocart/archive/v0.4.5.zip
+Download-URL: https://github.com/thespacedoctor/gocart/archive/v0.4.6.zip
 Author: David Young
 Author-email: d.r.young@qub.ac.uk
 License: MIT
 Keywords: astronomy
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `gocart-0.4.5/gocart.egg-info/SOURCES.txt` & `gocart-0.4.6/gocart.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -24,8 +24,9 @@
 gocart/commonutils/getpackagepath.py
 gocart/convert/__init__.py
 gocart/convert/aitoff.py
 gocart/convert/ascii.py
 gocart/convert/healpix2cart.py
 gocart/parsers/__init__.py
 gocart/parsers/lvk.py
+gocart/resources/package.mplstyle
 gocart/resources/plugins/gp_template.py
```

### Comparing `gocart-0.4.5/setup.py` & `gocart-0.4.6/setup.py`

 * *Files identical despite different names*

