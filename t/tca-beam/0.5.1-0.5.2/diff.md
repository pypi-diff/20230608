# Comparing `tmp/tca_beam-0.5.1.tar.gz` & `tmp/tca_beam-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tca_beam-0.5.1.tar", max compression
+gzip compressed data, was "tca_beam-0.5.2.tar", max compression
```

## Comparing `tca_beam-0.5.1.tar` & `tca_beam-0.5.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      143 2023-06-05 14:46:22.215862 tca_beam-0.5.1/README.md
--rw-r--r--   0        0        0      425 2023-06-07 20:54:47.052638 tca_beam-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      169 2023-06-05 13:50:29.564328 tca_beam-0.5.1/tca_beam/__init__.py
--rw-r--r--   0        0        0      311 2023-06-07 20:53:58.933860 tca_beam-0.5.1/tca_beam/config.py
--rw-r--r--   0        0        0     7152 2023-06-07 20:54:24.589965 tca_beam-0.5.1/tca_beam/tca_beam.py
--rw-r--r--   0        0        0      628 2023-06-07 19:24:52.000000 tca_beam-0.5.1/tca_beam/templates/AllPreviews.swift
--rw-r--r--   0        0        0       86 2023-06-07 17:31:44.668724 tca_beam-0.5.1/tca_beam/templates/OneFile.swift
--rw-r--r--   0        0        0       52 2023-06-05 09:23:16.046676 tca_beam-0.5.1/tca_beam/templates/TwoFile_ReducerPart.swift
--rw-r--r--   0        0        0       64 2023-06-04 21:52:01.190023 tca_beam-0.5.1/tca_beam/templates/TwoFile_ViewPart.swift
--rw-r--r--   0        0        0      723 2023-06-07 19:20:58.432700 tca_beam-0.5.1/tca_beam/templates/View.swift
--rw-r--r--   0        0        0      463 2023-06-04 22:08:47.296586 tca_beam-0.5.1/tca_beam/templates/ViewFeature.swift
--rw-r--r--   0        0        0      958 1970-01-01 00:00:00.000000 tca_beam-0.5.1/setup.py
--rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 tca_beam-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      143 2023-06-05 14:46:22.215862 tca_beam-0.5.2/README.md
+-rw-r--r--   0        0        0      425 2023-06-07 20:55:37.701870 tca_beam-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      169 2023-06-05 13:50:29.564328 tca_beam-0.5.2/tca_beam/__init__.py
+-rw-r--r--   0        0        0      311 2023-06-07 20:53:58.933860 tca_beam-0.5.2/tca_beam/config.py
+-rw-r--r--   0        0        0     7154 2023-06-07 20:55:30.855676 tca_beam-0.5.2/tca_beam/tca_beam.py
+-rw-r--r--   0        0        0      628 2023-06-07 19:24:52.000000 tca_beam-0.5.2/tca_beam/templates/AllPreviews.swift
+-rw-r--r--   0        0        0       86 2023-06-07 17:31:44.668724 tca_beam-0.5.2/tca_beam/templates/OneFile.swift
+-rw-r--r--   0        0        0       52 2023-06-05 09:23:16.046676 tca_beam-0.5.2/tca_beam/templates/TwoFile_ReducerPart.swift
+-rw-r--r--   0        0        0       64 2023-06-04 21:52:01.190023 tca_beam-0.5.2/tca_beam/templates/TwoFile_ViewPart.swift
+-rw-r--r--   0        0        0      723 2023-06-07 19:20:58.432700 tca_beam-0.5.2/tca_beam/templates/View.swift
+-rw-r--r--   0        0        0      463 2023-06-04 22:08:47.296586 tca_beam-0.5.2/tca_beam/templates/ViewFeature.swift
+-rw-r--r--   0        0        0      958 1970-01-01 00:00:00.000000 tca_beam-0.5.2/setup.py
+-rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 tca_beam-0.5.2/PKG-INFO
```

### Comparing `tca_beam-0.5.1/tca_beam/tca_beam.py` & `tca_beam-0.5.2/tca_beam/tca_beam.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 #  doesn't work either, doesn't even run locally!
 # from tca_beam import config
 
 # from config import BeamConfig
 # import config
 
-from config import *
+# from config import *
 
 beam_version = "(beam is not packaged so no version)"
 
 try:
     from tca_beam import __version__
     beam_version = __version__
 except ImportError:
```

### Comparing `tca_beam-0.5.1/tca_beam/templates/AllPreviews.swift` & `tca_beam-0.5.2/tca_beam/templates/AllPreviews.swift`

 * *Files identical despite different names*

### Comparing `tca_beam-0.5.1/tca_beam/templates/View.swift` & `tca_beam-0.5.2/tca_beam/templates/View.swift`

 * *Files identical despite different names*

### Comparing `tca_beam-0.5.1/setup.py` & `tca_beam-0.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['click>=8.1.3,<9.0.0', 'jinja2>=3.1.2,<4.0.0']
 
 entry_points = \
 {'console_scripts': ['tca-beam = tca_beam.tca_beam:start']}
 
 setup_kwargs = {
     'name': 'tca-beam',
-    'version': '0.5.1',
+    'version': '0.5.2',
     'description': 'Feature stub generation for The Composable Architecture',
     'long_description': 'TCA-beam, a helper for The Composable Architecture for creating Views and Reducers for new features.\n\nhttps://github.com/alexhunsley/tca-beam\n\n',
     'author': 'Alex Hunsley',
     'author_email': 'alex.hunsley@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `tca_beam-0.5.1/PKG-INFO` & `tca_beam-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tca-beam
-Version: 0.5.1
+Version: 0.5.2
 Summary: Feature stub generation for The Composable Architecture
 Author: Alex Hunsley
 Author-email: alex.hunsley@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

