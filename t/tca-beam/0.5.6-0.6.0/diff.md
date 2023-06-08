# Comparing `tmp/tca_beam-0.5.6.tar.gz` & `tmp/tca_beam-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tca_beam-0.5.6.tar", max compression
+gzip compressed data, was "tca_beam-0.6.0.tar", max compression
```

## Comparing `tca_beam-0.5.6.tar` & `tca_beam-0.6.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rw-r--r--   0        0        0      143 2023-06-05 14:46:22.215862 tca_beam-0.5.6/README.md
--rw-r--r--   0        0        0      467 2023-06-08 12:45:37.867571 tca_beam-0.5.6/pyproject.toml
--rw-r--r--   0        0        0      173 2023-06-08 15:05:54.275604 tca_beam-0.5.6/tca_beam/__init__.py
--rw-r--r--   0        0        0      282 2023-06-08 12:31:34.393036 tca_beam-0.5.6/tca_beam/config.py
--rw-r--r--   0        0        0      273 2023-06-08 12:35:53.205826 tca_beam-0.5.6/tca_beam/helpers.py
--rw-r--r--   0        0        0     2391 2023-06-08 12:41:09.499457 tca_beam-0.5.6/tca_beam/run.py
--rw-r--r--   0        0        0     2616 2023-06-08 15:08:01.131913 tca_beam-0.5.6/tca_beam/tca_beam.py
--rw-r--r--   0        0        0     1615 2023-06-08 12:38:17.485233 tca_beam-0.5.6/tca_beam/template_rendering.py
--rw-r--r--   0        0        0      628 2023-06-07 19:24:52.000000 tca_beam-0.5.6/tca_beam/templates/AllPreviews.swift
--rw-r--r--   0        0        0       86 2023-06-07 17:31:44.668724 tca_beam-0.5.6/tca_beam/templates/OneFile.swift
--rw-r--r--   0        0        0       52 2023-06-05 09:23:16.046676 tca_beam-0.5.6/tca_beam/templates/TwoFile_ReducerPart.swift
--rw-r--r--   0        0        0       64 2023-06-04 21:52:01.190023 tca_beam-0.5.6/tca_beam/templates/TwoFile_ViewPart.swift
--rw-r--r--   0        0        0      723 2023-06-07 19:20:58.432700 tca_beam-0.5.6/tca_beam/templates/View.swift
--rw-r--r--   0        0        0      463 2023-06-04 22:08:47.296586 tca_beam-0.5.6/tca_beam/templates/ViewFeature.swift
--rw-r--r--   0        0        0      958 1970-01-01 00:00:00.000000 tca_beam-0.5.6/setup.py
--rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 tca_beam-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0      143 2023-06-05 14:46:22.215862 tca_beam-0.6.0/README.md
+-rw-r--r--   0        0        0      467 2023-06-08 19:49:26.331860 tca_beam-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      173 2023-06-08 15:05:54.275604 tca_beam-0.6.0/tca_beam/__init__.py
+-rw-r--r--   0        0        0     2310 2023-06-08 19:47:14.919545 tca_beam-0.6.0/tca_beam/config.py
+-rw-r--r--   0        0        0      391 2023-06-08 19:32:23.316107 tca_beam-0.6.0/tca_beam/helpers.py
+-rw-r--r--   0        0        0     3378 2023-06-08 19:22:18.129289 tca_beam-0.6.0/tca_beam/run.py
+-rw-r--r--   0        0        0     2305 2023-06-08 19:19:20.544259 tca_beam-0.6.0/tca_beam/settings.py
+-rw-r--r--   0        0        0     3404 2023-06-08 19:20:03.772655 tca_beam-0.6.0/tca_beam/tca_beam.py
+-rw-r--r--   0        0        0     1618 2023-06-08 19:32:34.191285 tca_beam-0.6.0/tca_beam/template_rendering.py
+-rw-r--r--   0        0        0      281 2023-06-08 19:47:29.314314 tca_beam-0.6.0/tca_beam/templates/.beam-settings.toml
+-rw-r--r--   0        0        0      628 2023-06-07 19:24:52.000000 tca_beam-0.6.0/tca_beam/templates/AllPreviews.swift
+-rw-r--r--   0        0        0       86 2023-06-07 17:31:44.668724 tca_beam-0.6.0/tca_beam/templates/OneFile.swift
+-rw-r--r--   0        0        0       52 2023-06-05 09:23:16.046676 tca_beam-0.6.0/tca_beam/templates/TwoFile_ReducerPart.swift
+-rw-r--r--   0        0        0       64 2023-06-04 21:52:01.190023 tca_beam-0.6.0/tca_beam/templates/TwoFile_ViewPart.swift
+-rw-r--r--   0        0        0      723 2023-06-07 19:20:58.432700 tca_beam-0.6.0/tca_beam/templates/View.swift
+-rw-r--r--   0        0        0      463 2023-06-04 22:08:47.296586 tca_beam-0.6.0/tca_beam/templates/ViewFeature.swift
+-rw-r--r--   0        0        0      958 1970-01-01 00:00:00.000000 tca_beam-0.6.0/setup.py
+-rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 tca_beam-0.6.0/PKG-INFO
```

### Comparing `tca_beam-0.5.6/tca_beam/run.py` & `tca_beam-0.6.0/tca_beam/run.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from .template_rendering import *
 
+
 def process_template(config, feature_name):
     dbg(f"start process_template, config = {config}, sub_dirs = {config.sub_dirs}")
 
     substitutions = {
         'viewName': f"{feature_name}View",
         'featureName': f"{feature_name}ViewFeature"
     }
@@ -20,19 +21,33 @@
 
     template_renders = []
 
     target_dir = f"{feature_name}Feature" if config.sub_dirs else "."
 
     dbg(f"just made target_dir: {config.target_dir}, and sub_dirs == {config.sub_dirs}")
     if config.two_files:
-        template_renders.append(TemplateRender(f"{feature_name}ViewFeature.swift", config.jinja_env.get_template('TwoFile_ReducerPart.swift'), target_dir))
-        template_renders.append(TemplateRender(f"{feature_name}View.swift", config.jinja_env.get_template('TwoFile_ViewPart.swift'), target_dir))
+        # could do replacement inside TemplateRender? Or make method helper in this file, more likely
+        reducer_filename = config.permanent_settings.two_files_reducer_part_filename.replace("{{featureName}}", feature_name)
+        dbg(f"Made RF: {reducer_filename}")
+        template_renders.append(TemplateRender(reducer_filename,
+                                               config.jinja_env.get_template('TwoFile_ReducerPart.swift'),
+                                               target_dir))
+
+        view_filename = config.permanent_settings.two_files_view_part_filename.replace("{{featureName}}", feature_name)
+        dbg(f"Made VF: {view_filename}")
+        template_renders.append(TemplateRender(view_filename,
+                                               config.jinja_env.get_template('TwoFile_ViewPart.swift'),
+                                               target_dir))
     else:
+        one_file_filename = config.permanent_settings.one_file_filename.replace("{{featureName}}", feature_name)
+        dbg(f"Made OFF: {one_file_filename}")
         # for reducer + view in one file, we append just 'View' to feature name
-        template_renders.append(TemplateRender(f"{feature_name}View.swift", config.jinja_env.get_template('OneFile.swift'), target_dir))
+        template_renders.append(TemplateRender(one_file_filename,
+                                               config.jinja_env.get_template('OneFile.swift'),
+                                               target_dir))
 
     step_name = f"Feature '{feature_name}':"
     render_templates(config, template_renders, substitutions, step_name)
 
 
 def generate_all_preview(config):
 
@@ -43,15 +58,18 @@
         all_previews_substitutions.append({
             'viewName': f"{feature_name}View",
             'featureName': f"{feature_name}ViewFeature"
         })
 
     substitutions_all_previews = { 'allFeatures': all_previews_substitutions}
 
-    template_render = TemplateRender(f"AllPreviews.swift", config.jinja_env.get_template('AllPreviews.swift'))
+    preview_all_filename = config.permanent_settings.preview_all_filename.replace("{{featureName}}", feature_name)
+
+    template_render = TemplateRender(preview_all_filename,
+                                     config.jinja_env.get_template('AllPreviews.swift'))
 
     render_templates(config, [template_render], substitutions_all_previews, 'Preview for all features:')
 
 
 def run(config):
     for feature_name in config.feature_names:
         process_template(config, feature_name)
```

### Comparing `tca_beam-0.5.6/tca_beam/tca_beam.py` & `tca_beam-0.6.0/tca_beam/tca_beam.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-import sys
 from jinja2 import Environment, FileSystemLoader
 import click
-
-from .config import BeamConfig
-from .template_rendering import *
+from .config import BeamConfig, PermanentSettings
 from .run import run
+from .settings import *
 
 beam_version = "(no version because beam is not packaged)"
 
 try:
     from tca_beam import __version__
     beam_version = __version__
 except ImportError:
@@ -24,37 +22,51 @@
 # -[x] make script use abs path to the templates, no chdir!
 # -[x] --dry-run
 
 # For docs:
 #  tca-beam won't complain if the output_dir already exists, regardless of force_overwrite flag (which only applies to files).
 #
 
+# When you're testing and playing with beam, it might be tempting to set up a host xcode project with a _link_ to a folder
+# where you are generating the files with beam.
+# However, Xcode however won't add these files to any target (it's how linked folders work), so you're probably better off
+# just adding a folder group to your project (in the usual way) after you've generated the files with beam.
+
 
 @click.command(no_args_is_help=True)
 @click.option('--two-files', is_flag=True, help="Put view and reducer into separate files")
 @click.option('--sub-dirs', is_flag=True, help="Put each feature in a sub-directory")
 @click.option('--preview-all', is_flag=True, help="Generate a single View that previews all feature Views")
 @click.option('--output-dir', default='.', help="Output directory (defaults to current dir)")
 @click.option('--force-overwrite', is_flag=True, help="Force overwriting any existing files")
 @click.option('--dry-run', is_flag=True, help="Don't generate files, just preview any actions")
+@click.option('--customise-settings', is_flag=True, help="Generate a user-editable file to tweak file naming settings.")
 @click.option('--version', is_flag=True, help="Print version and exit")
 @click.argument('feature_names', nargs=-1)
-def start(two_files, sub_dirs, preview_all, output_dir, force_overwrite, dry_run, version, feature_names):
+def start(two_files, sub_dirs, preview_all, output_dir, force_overwrite, dry_run, customise_settings, version, feature_names):
+
+    if customise_settings:
+        personalize_permanent_settings()
+        sys.exit(0)
+
+    permanent_settings = load_permanent_settings()
+    dbg(f"Settings: {permanent_settings}")
 
     if version:
         p(beam_version)
         sys.exit(0)
 
     script_dir = os.path.abspath(os.path.dirname(__file__))
 
     templates_path = make_abs_path('templates')
     file_loader = FileSystemLoader(templates_path)
     jinja_env = Environment(loader=file_loader)
 
-    config = BeamConfig(script_dir, output_dir, jinja_env, two_files, sub_dirs, preview_all, output_dir, force_overwrite, dry_run, feature_names)
+    config = BeamConfig(PermanentSettings(permanent_settings), script_dir, output_dir, jinja_env, two_files, sub_dirs, preview_all,
+                        output_dir, force_overwrite, dry_run, feature_names)
 
     if len(feature_names) < 1:
         p()
         p("Please give one or more feature name arguments (after any option flags).")
         p()
 
         echo = click.echo
```

### Comparing `tca_beam-0.5.6/tca_beam/template_rendering.py` & `tca_beam-0.6.0/tca_beam/template_rendering.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import sys
 from collections import namedtuple
 from pathlib import Path
 from .helpers import *
 
 TemplateRender = namedtuple('TemplateRender', ['render_file', 'template', 'target_dir'],
                             defaults=['', '', '.'])
 
@@ -28,19 +29,19 @@
         filepath = abs_directory / filename
 
         p(f"{console_prefix}   Creating file {filepath}")
 
         if not config.dry_run:
             if os.path.isdir(filepath):
                 error(f'A directory named "{filepath}" already exists, refusing to overwrite.')
-                error()
+                p()
                 sys.exit(1)
 
             if not config.force_overwrite and os.path.isfile(filepath):
                 error(f'A file named "{filepath}" already exists, refusing to overwrite. Use --force-overwrite to suppress this error.')
-                error()
+                p()
                 sys.exit(1)
 
             abs_directory.mkdir(parents=True, exist_ok=True)
 
             with open(filepath, 'w') as f:
                 f.write(stub_contents + '\n')
```

### Comparing `tca_beam-0.5.6/tca_beam/templates/AllPreviews.swift` & `tca_beam-0.6.0/tca_beam/templates/AllPreviews.swift`

 * *Files identical despite different names*

### Comparing `tca_beam-0.5.6/tca_beam/templates/View.swift` & `tca_beam-0.6.0/tca_beam/templates/View.swift`

 * *Files identical despite different names*

### Comparing `tca_beam-0.5.6/setup.py` & `tca_beam-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['click>=8.1.3,<9.0.0', 'jinja2>=3.1.2,<4.0.0']
 
 entry_points = \
 {'console_scripts': ['tca-beam = tca_beam.tca_beam:start']}
 
 setup_kwargs = {
     'name': 'tca-beam',
-    'version': '0.5.6',
+    'version': '0.6.0',
     'description': 'Feature stub generation for The Composable Architecture',
     'long_description': 'TCA-beam, a helper for The Composable Architecture for creating Views and Reducers for new features.\n\nhttps://github.com/alexhunsley/tca-beam\n\n',
     'author': 'Alex Hunsley',
     'author_email': 'alex.hunsley@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `tca_beam-0.5.6/PKG-INFO` & `tca_beam-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tca-beam
-Version: 0.5.6
+Version: 0.6.0
 Summary: Feature stub generation for The Composable Architecture
 Author: Alex Hunsley
 Author-email: alex.hunsley@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

