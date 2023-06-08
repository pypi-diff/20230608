# Comparing `tmp/inventree-brother-plugin-0.6.0.tar.gz` & `tmp/inventree-brother-plugin-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/inventree-brother-plugin-0.6.0.tar", last modified: Fri Jan  6 01:58:39 2023, max compression
+gzip compressed data, was "dist/inventree-brother-plugin-0.6.1.tar", last modified: Thu Jun  8 09:53:41 2023, max compression
```

## Comparing `inventree-brother-plugin-0.6.0.tar` & `inventree-brother-plugin-0.6.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 01:58:39.000000 inventree-brother-plugin-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-01-06 01:58:29.000000 inventree-brother-plugin-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-01-06 01:58:39.000000 inventree-brother-plugin-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-01-06 01:58:29.000000 inventree-brother-plugin-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 01:58:39.000000 inventree-brother-plugin-0.6.0/inventree_brother/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-06 01:58:29.000000 inventree-brother-plugin-0.6.0/inventree_brother/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-01-06 01:58:29.000000 inventree-brother-plugin-0.6.0/inventree_brother/brother_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-01-06 01:58:29.000000 inventree-brother-plugin-0.6.0/inventree_brother/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 01:58:39.000000 inventree-brother-plugin-0.6.0/inventree_brother_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-01-06 01:58:39.000000 inventree-brother-plugin-0.6.0/inventree_brother_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-01-06 01:58:39.000000 inventree-brother-plugin-0.6.0/inventree_brother_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-06 01:58:39.000000 inventree-brother-plugin-0.6.0/inventree_brother_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-01-06 01:58:39.000000 inventree-brother-plugin-0.6.0/inventree_brother_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-06 01:58:39.000000 inventree-brother-plugin-0.6.0/inventree_brother_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-06 01:58:39.000000 inventree-brother-plugin-0.6.0/inventree_brother_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-01-06 01:58:39.000000 inventree-brother-plugin-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-01-06 01:58:29.000000 inventree-brother-plugin-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:53:41.000000 inventree-brother-plugin-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-08 09:53:33.000000 inventree-brother-plugin-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-08 09:53:41.000000 inventree-brother-plugin-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-08 09:53:33.000000 inventree-brother-plugin-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:53:41.000000 inventree-brother-plugin-0.6.1/inventree_brother/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:53:33.000000 inventree-brother-plugin-0.6.1/inventree_brother/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-06-08 09:53:33.000000 inventree-brother-plugin-0.6.1/inventree_brother/brother_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-08 09:53:33.000000 inventree-brother-plugin-0.6.1/inventree_brother/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:53:41.000000 inventree-brother-plugin-0.6.1/inventree_brother_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-08 09:53:41.000000 inventree-brother-plugin-0.6.1/inventree_brother_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-08 09:53:41.000000 inventree-brother-plugin-0.6.1/inventree_brother_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 09:53:41.000000 inventree-brother-plugin-0.6.1/inventree_brother_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-08 09:53:41.000000 inventree-brother-plugin-0.6.1/inventree_brother_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-08 09:53:41.000000 inventree-brother-plugin-0.6.1/inventree_brother_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-08 09:53:41.000000 inventree-brother-plugin-0.6.1/inventree_brother_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-08 09:53:41.000000 inventree-brother-plugin-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-08 09:53:33.000000 inventree-brother-plugin-0.6.1/setup.py
```

### Comparing `inventree-brother-plugin-0.6.0/LICENSE` & `inventree-brother-plugin-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `inventree-brother-plugin-0.6.0/PKG-INFO` & `inventree-brother-plugin-0.6.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: inventree-brother-plugin
-Version: 0.6.0
-Summary: Brother label printer plugin for InvenTree
-Home-page: https://github.com/inventree/inventree-brother-plugin
-Author: Oliver Walters
-Author-email: oliver.henry.walters@gmail.com
-License: MIT
-Keywords: inventree label printer printing inventory
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 ![PEP](https://github.com/inventree/inventree-python/actions/workflows/pep.yaml/badge.svg)
 
 
 # inventree-brother-plugin
 
 A label printing plugin for [InvenTree](https://inventree.org), which provides support for the [Brother label printers](https://www.brother.com.au/en/products/all-labellers/labellers).
@@ -31,10 +18,22 @@
 
 Or, add to your `plugins.txt` file to install automatically using the `invoke install` command:
 
 ```
 inventree-brother-plugin
 ```
  
+### Debian / Ubuntu requirements
+
+The following command can be used to install all OS-requirements on Debian / Ubuntu-based distros:
+```bash
+apt install build-essential libpoppler-cpp-dev pkg-config poppler-utils
+```
+
+You might also need the following Python packages:
+```bash
+pip install pdf-info python-poppler
+```
+
 ## Configuration Options
 
 **TODO**
```

### Comparing `inventree-brother-plugin-0.6.0/inventree_brother/brother_plugin.py` & `inventree-brother-plugin-0.6.1/inventree_brother/brother_plugin.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,25 +4,28 @@
 """
 
 # Required brother_ql libs
 from brother_ql.conversion import convert
 from brother_ql.raster import BrotherQLRaster
 from brother_ql.backends.helpers import send
 from brother_ql.models import ALL_MODELS
-from brother_ql.labels import ALL_LABELS
+from brother_ql.labels import ALL_LABELS, FormFactor
 
 # translation
 from django.utils.translation import ugettext_lazy as _
 
 from inventree_brother.version import BROTHER_PLUGIN_VERSION
 
 # InvenTree plugin libs
 from plugin import InvenTreePlugin
 from plugin.mixins import LabelPrintingMixin, SettingsMixin
 
+# Image library
+from PIL import ImageOps
+
 
 def get_model_choices():
     """
     Returns a list of available printer models
     """
 
     return [(model.name, model.name) for model in ALL_MODELS]
@@ -100,41 +103,67 @@
 
     def print_label(self, **kwargs):
         """
         Send the label to the printer
         """
 
         # TODO: Add padding around the provided image, otherwise the label does not print correctly
+        # ^ Why? The wording in the underlying brother_ql library ('dots_printable') seems to suggest
+        # at least that area is fully printable.
         # TODO: Improve label auto-scaling based on provided width and height information
 
         # Extract width (x) and height (y) information
         # width = kwargs['width']
         # height = kwargs['height']
+        # ^ currently this width and height are those of the label template (before conversion to PDF
+        # and PNG) and are of little use
 
         # Extract image from the provided kwargs
         label_image = kwargs['png_file']
 
         # Read settings
         model = self.get_setting('MODEL')
         ip_address = self.get_setting('IP_ADDRESS')
-        label = self.get_setting('LABEL')
+        media_type = self.get_setting('LABEL')
+
+        # Get specifications of media type
+        media_specs = None
+        for label_specs in ALL_LABELS:
+            if label_specs.identifier == media_type:
+                media_specs = label_specs
+
+        try:
+            # Resize image if media type is a die cut label (the brother_ql library only accepts images
+            # with a specific size in that case)
+            # TODO: Make it generic for all media types
+            # TODO: Add GUI settings to configure scaling and margins
+            if media_specs.form_factor in [FormFactor.DIE_CUT, FormFactor.ROUND_DIE_CUT]:
+                # Scale image to fit the entire printable area and pad with whitespace (while preserving aspect ratio)
+                printable_image = ImageOps.pad(label_image, media_specs.dots_printable, color="white")
+            else:
+                # Just leave image as-is
+                printable_image = label_image
+        except AttributeError as e:
+            raise AttributeError("Could not find specifications of label media type '%s'" % media_type) from e
+        except Exception as e:
+            raise e
 
         # Check if red labels used
-        if label in ['62red']:
+        if media_type in ['62red']:
             red = True
         else:
             red = False
 
         printer = BrotherQLRaster(model=model)
 
         # Generate instructions for printing
         params = {
             'qlr': printer,
-            'images': [label_image],
-            'label': label,
+            'images': [printable_image],
+            'label': media_type,
             'cut': self.get_setting('AUTO_CUT'),
             'rotate': self.get_setting('ROTATION'),
             'compress': self.get_setting('COMPRESSION'),
             'hq': self.get_setting('HQ'),
             'red': red,
         }
```

### Comparing `inventree-brother-plugin-0.6.0/setup.py` & `inventree-brother-plugin-0.6.1/setup.py`

 * *Files identical despite different names*

