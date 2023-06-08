# Comparing `tmp/tca_beam-0.6.0.tar.gz` & `tmp/tca_beam-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tca_beam-0.6.0.tar", max compression
+gzip compressed data, was "tca_beam-0.6.1.tar", max compression
```

## Comparing `tca_beam-0.6.0.tar` & `tca_beam-0.6.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      143 2023-06-05 14:46:22.215862 tca_beam-0.6.0/README.md
--rw-r--r--   0        0        0      467 2023-06-08 19:49:26.331860 tca_beam-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      173 2023-06-08 15:05:54.275604 tca_beam-0.6.0/tca_beam/__init__.py
--rw-r--r--   0        0        0     2310 2023-06-08 19:47:14.919545 tca_beam-0.6.0/tca_beam/config.py
--rw-r--r--   0        0        0      391 2023-06-08 19:32:23.316107 tca_beam-0.6.0/tca_beam/helpers.py
--rw-r--r--   0        0        0     3378 2023-06-08 19:22:18.129289 tca_beam-0.6.0/tca_beam/run.py
--rw-r--r--   0        0        0     2305 2023-06-08 19:19:20.544259 tca_beam-0.6.0/tca_beam/settings.py
--rw-r--r--   0        0        0     3404 2023-06-08 19:20:03.772655 tca_beam-0.6.0/tca_beam/tca_beam.py
--rw-r--r--   0        0        0     1618 2023-06-08 19:32:34.191285 tca_beam-0.6.0/tca_beam/template_rendering.py
--rw-r--r--   0        0        0      281 2023-06-08 19:47:29.314314 tca_beam-0.6.0/tca_beam/templates/.beam-settings.toml
--rw-r--r--   0        0        0      628 2023-06-07 19:24:52.000000 tca_beam-0.6.0/tca_beam/templates/AllPreviews.swift
--rw-r--r--   0        0        0       86 2023-06-07 17:31:44.668724 tca_beam-0.6.0/tca_beam/templates/OneFile.swift
--rw-r--r--   0        0        0       52 2023-06-05 09:23:16.046676 tca_beam-0.6.0/tca_beam/templates/TwoFile_ReducerPart.swift
--rw-r--r--   0        0        0       64 2023-06-04 21:52:01.190023 tca_beam-0.6.0/tca_beam/templates/TwoFile_ViewPart.swift
--rw-r--r--   0        0        0      723 2023-06-07 19:20:58.432700 tca_beam-0.6.0/tca_beam/templates/View.swift
--rw-r--r--   0        0        0      463 2023-06-04 22:08:47.296586 tca_beam-0.6.0/tca_beam/templates/ViewFeature.swift
--rw-r--r--   0        0        0      958 1970-01-01 00:00:00.000000 tca_beam-0.6.0/setup.py
--rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 tca_beam-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      143 2023-06-05 14:46:22.215862 tca_beam-0.6.1/README.md
+-rw-r--r--   0        0        0      467 2023-06-08 20:10:28.778184 tca_beam-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      173 2023-06-08 15:05:54.275604 tca_beam-0.6.1/tca_beam/__init__.py
+-rw-r--r--   0        0        0     2310 2023-06-08 19:47:14.919545 tca_beam-0.6.1/tca_beam/config.py
+-rw-r--r--   0        0        0      391 2023-06-08 19:32:23.316107 tca_beam-0.6.1/tca_beam/helpers.py
+-rw-r--r--   0        0        0     3378 2023-06-08 19:22:18.129289 tca_beam-0.6.1/tca_beam/run.py
+-rw-r--r--   0        0        0     2403 2023-06-08 20:06:36.255252 tca_beam-0.6.1/tca_beam/settings.py
+-rw-r--r--   0        0        0     3404 2023-06-08 19:20:03.772655 tca_beam-0.6.1/tca_beam/tca_beam.py
+-rw-r--r--   0        0        0     1618 2023-06-08 19:32:34.191285 tca_beam-0.6.1/tca_beam/template_rendering.py
+-rw-r--r--   0        0        0      278 2023-06-08 19:54:34.492699 tca_beam-0.6.1/tca_beam/templates/.beam-settings.toml
+-rw-r--r--   0        0        0      628 2023-06-07 19:24:52.000000 tca_beam-0.6.1/tca_beam/templates/AllPreviews.swift
+-rw-r--r--   0        0        0       86 2023-06-07 17:31:44.668724 tca_beam-0.6.1/tca_beam/templates/OneFile.swift
+-rw-r--r--   0        0        0       52 2023-06-05 09:23:16.046676 tca_beam-0.6.1/tca_beam/templates/TwoFile_ReducerPart.swift
+-rw-r--r--   0        0        0       64 2023-06-04 21:52:01.190023 tca_beam-0.6.1/tca_beam/templates/TwoFile_ViewPart.swift
+-rw-r--r--   0        0        0      723 2023-06-07 19:20:58.432700 tca_beam-0.6.1/tca_beam/templates/View.swift
+-rw-r--r--   0        0        0      463 2023-06-04 22:08:47.296586 tca_beam-0.6.1/tca_beam/templates/ViewFeature.swift
+-rw-r--r--   0        0        0      958 1970-01-01 00:00:00.000000 tca_beam-0.6.1/setup.py
+-rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 tca_beam-0.6.1/PKG-INFO
```

### Comparing `tca_beam-0.6.0/tca_beam/config.py` & `tca_beam-0.6.1/tca_beam/config.py`

 * *Files identical despite different names*

### Comparing `tca_beam-0.6.0/tca_beam/run.py` & `tca_beam-0.6.1/tca_beam/run.py`

 * *Files identical despite different names*

### Comparing `tca_beam-0.6.0/tca_beam/settings.py` & `tca_beam-0.6.1/tca_beam/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,17 +27,20 @@
         p("If you want to generate the settings file again from defaults, please delete that existing file first.")
         p()
         sys.exit(1)
 
     # Copy the settings file
     shutil.copyfile(default_settings_path, destination_settings_path)
 
-    p(f"I've copied default settings to {destination_settings_path}.")
+    p()
+    p(f"I've copied default settings to '{destination_settings_path}'.")
     p(f"Please edit this file with your favourite text editor.")
     p()
+    p("Note that you can later delete this file to go back to the defaults.")
+    p("")
     sys.exit(0)
 
 
 def load_permanent_settings() -> Optional[ConfigParser]:
     """
     Loads the user's custom settings if they exist, otherwise loads the default settings.
     Returns a ConfigParser object, or None if no settings file is found.
```

### Comparing `tca_beam-0.6.0/tca_beam/tca_beam.py` & `tca_beam-0.6.1/tca_beam/tca_beam.py`

 * *Files identical despite different names*

### Comparing `tca_beam-0.6.0/tca_beam/template_rendering.py` & `tca_beam-0.6.1/tca_beam/template_rendering.py`

 * *Files identical despite different names*

### Comparing `tca_beam-0.6.0/tca_beam/templates/AllPreviews.swift` & `tca_beam-0.6.1/tca_beam/templates/AllPreviews.swift`

 * *Files identical despite different names*

### Comparing `tca_beam-0.6.0/tca_beam/templates/View.swift` & `tca_beam-0.6.1/tca_beam/templates/View.swift`

 * *Files identical despite different names*

### Comparing `tca_beam-0.6.0/setup.py` & `tca_beam-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['click>=8.1.3,<9.0.0', 'jinja2>=3.1.2,<4.0.0']
 
 entry_points = \
 {'console_scripts': ['tca-beam = tca_beam.tca_beam:start']}
 
 setup_kwargs = {
     'name': 'tca-beam',
-    'version': '0.6.0',
+    'version': '0.6.1',
     'description': 'Feature stub generation for The Composable Architecture',
     'long_description': 'TCA-beam, a helper for The Composable Architecture for creating Views and Reducers for new features.\n\nhttps://github.com/alexhunsley/tca-beam\n\n',
     'author': 'Alex Hunsley',
     'author_email': 'alex.hunsley@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `tca_beam-0.6.0/PKG-INFO` & `tca_beam-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tca-beam
-Version: 0.6.0
+Version: 0.6.1
 Summary: Feature stub generation for The Composable Architecture
 Author: Alex Hunsley
 Author-email: alex.hunsley@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

