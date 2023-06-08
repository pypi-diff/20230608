# Comparing `tmp/phoebusgen-2.6.0.tar.gz` & `tmp/phoebusgen-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phoebusgen-2.6.0.tar", last modified: Mon Jun  5 23:39:14 2023, max compression
+gzip compressed data, was "phoebusgen-2.6.1.tar", last modified: Thu Jun  8 04:39:42 2023, max compression
```

## Comparing `phoebusgen-2.6.0.tar` & `phoebusgen-2.6.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:39:14.021391 phoebusgen-2.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    17987 2023-06-05 23:39:02.000000 phoebusgen-2.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-05 23:39:02.000000 phoebusgen-2.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-06-05 23:39:14.021391 phoebusgen-2.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-06-05 23:39:02.000000 phoebusgen-2.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:39:14.021391 phoebusgen-2.6.0/phoebusgen/
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-06-05 23:39:02.000000 phoebusgen-2.6.0/phoebusgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-06-05 23:39:02.000000 phoebusgen-2.6.0/phoebusgen/_shared_property_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-05 23:39:14.021391 phoebusgen-2.6.0/phoebusgen/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:39:14.021391 phoebusgen-2.6.0/phoebusgen/config/
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-06-05 23:39:02.000000 phoebusgen-2.6.0/phoebusgen/config/classes.bcf
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-05 23:39:02.000000 phoebusgen-2.6.0/phoebusgen/config/color.def
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-05 23:39:02.000000 phoebusgen-2.6.0/phoebusgen/config/font.def
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:39:14.021391 phoebusgen-2.6.0/phoebusgen/screen/
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-05 23:39:02.000000 phoebusgen-2.6.0/phoebusgen/screen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-06-05 23:39:02.000000 phoebusgen-2.6.0/phoebusgen/screen/screen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:39:14.021391 phoebusgen-2.6.0/phoebusgen/widget/
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-05 23:39:02.000000 phoebusgen-2.6.0/phoebusgen/widget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    65736 2023-06-05 23:39:02.000000 phoebusgen-2.6.0/phoebusgen/widget/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-06-05 23:39:02.000000 phoebusgen-2.6.0/phoebusgen/widget/widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    27640 2023-06-05 23:39:02.000000 phoebusgen-2.6.0/phoebusgen/widget/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:39:14.017391 phoebusgen-2.6.0/phoebusgen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-06-05 23:39:14.000000 phoebusgen-2.6.0/phoebusgen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-05 23:39:14.000000 phoebusgen-2.6.0/phoebusgen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 23:39:14.000000 phoebusgen-2.6.0/phoebusgen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-05 23:39:14.000000 phoebusgen-2.6.0/phoebusgen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 23:39:02.000000 phoebusgen-2.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-05 23:39:14.021391 phoebusgen-2.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-05 23:39:02.000000 phoebusgen-2.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:39:14.021391 phoebusgen-2.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-06-05 23:39:02.000000 phoebusgen-2.6.0/tests/test_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)    10648 2023-06-05 23:39:02.000000 phoebusgen-2.6.0/tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    22198 2023-06-05 23:39:02.000000 phoebusgen-2.6.0/tests/test_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)    81180 2023-06-05 23:39:02.000000 phoebusgen-2.6.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 04:39:42.207512 phoebusgen-2.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    17987 2023-06-08 04:39:29.000000 phoebusgen-2.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-08 04:39:29.000000 phoebusgen-2.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-06-08 04:39:42.207512 phoebusgen-2.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-06-08 04:39:29.000000 phoebusgen-2.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 04:39:42.207512 phoebusgen-2.6.1/phoebusgen/
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-06-08 04:39:29.000000 phoebusgen-2.6.1/phoebusgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-06-08 04:39:29.000000 phoebusgen-2.6.1/phoebusgen/_shared_property_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-08 04:39:42.207512 phoebusgen-2.6.1/phoebusgen/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 04:39:42.207512 phoebusgen-2.6.1/phoebusgen/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-06-08 04:39:29.000000 phoebusgen-2.6.1/phoebusgen/config/classes.bcf
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-08 04:39:29.000000 phoebusgen-2.6.1/phoebusgen/config/color.def
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-08 04:39:29.000000 phoebusgen-2.6.1/phoebusgen/config/font.def
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 04:39:42.207512 phoebusgen-2.6.1/phoebusgen/screen/
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-08 04:39:29.000000 phoebusgen-2.6.1/phoebusgen/screen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-06-08 04:39:29.000000 phoebusgen-2.6.1/phoebusgen/screen/screen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 04:39:42.207512 phoebusgen-2.6.1/phoebusgen/widget/
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-08 04:39:29.000000 phoebusgen-2.6.1/phoebusgen/widget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67600 2023-06-08 04:39:29.000000 phoebusgen-2.6.1/phoebusgen/widget/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-06-08 04:39:29.000000 phoebusgen-2.6.1/phoebusgen/widget/widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27640 2023-06-08 04:39:29.000000 phoebusgen-2.6.1/phoebusgen/widget/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 04:39:42.203512 phoebusgen-2.6.1/phoebusgen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-06-08 04:39:42.000000 phoebusgen-2.6.1/phoebusgen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-08 04:39:42.000000 phoebusgen-2.6.1/phoebusgen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 04:39:42.000000 phoebusgen-2.6.1/phoebusgen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-08 04:39:42.000000 phoebusgen-2.6.1/phoebusgen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 04:39:29.000000 phoebusgen-2.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-08 04:39:42.207512 phoebusgen-2.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-08 04:39:29.000000 phoebusgen-2.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 04:39:42.207512 phoebusgen-2.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-06-08 04:39:29.000000 phoebusgen-2.6.1/tests/test_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10648 2023-06-08 04:39:29.000000 phoebusgen-2.6.1/tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22198 2023-06-08 04:39:29.000000 phoebusgen-2.6.1/tests/test_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81180 2023-06-08 04:39:29.000000 phoebusgen-2.6.1/versioneer.py
```

### Comparing `phoebusgen-2.6.0/LICENSE` & `phoebusgen-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.6.0/PKG-INFO` & `phoebusgen-2.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phoebusgen
-Version: 2.6.0
+Version: 2.6.1
 Summary: Control screen generator for Phoebus
 Home-page: https://github.com/tynanford/phoebusgen
 Author: Tynan Ford
 Author-email: tford@lbl.gov
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
```

### Comparing `phoebusgen-2.6.0/README.md` & `phoebusgen-2.6.1/README.md`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.6.0/phoebusgen/__init__.py` & `phoebusgen-2.6.1/phoebusgen/__init__.py`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.6.0/phoebusgen/_shared_property_helpers.py` & `phoebusgen-2.6.1/phoebusgen/_shared_property_helpers.py`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.6.0/phoebusgen/config/classes.bcf` & `phoebusgen-2.6.1/phoebusgen/config/classes.bcf`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.6.0/phoebusgen/config/color.def` & `phoebusgen-2.6.1/phoebusgen/config/color.def`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.6.0/phoebusgen/config/font.def` & `phoebusgen-2.6.1/phoebusgen/config/font.def`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.6.0/phoebusgen/screen/__init__.py` & `phoebusgen-2.6.1/phoebusgen/screen/__init__.py`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.6.0/phoebusgen/screen/screen.py` & `phoebusgen-2.6.1/phoebusgen/screen/screen.py`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.6.0/phoebusgen/widget/__init__.py` & `phoebusgen-2.6.1/phoebusgen/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.6.0/phoebusgen/widget/properties.py` & `phoebusgen-2.6.1/phoebusgen/widget/properties.py`

 * *Files 3% similar despite different names*

```diff
@@ -705,31 +705,38 @@
         Add stretch to fit property to widget
 
         :param val: Stretch widget to fit?
         """
         self._shared.boolean_property(self.root, 'stretch_image', val)
 
 class _Actions(object):
-    def _add_action(self, action_type, description, args, macros=None):
+    def _add_action(self, action_type, description, args, isScript, macros=None):
         root_action = self.root.find('actions')
         if root_action is None:
             root_action = SubElement(self.root, 'actions')
         action = SubElement(root_action, 'action')
         action.attrib['type'] = action_type
         sub = SubElement(action, 'description')
         sub.text = str(description)
         if macros:
             if not isinstance(macros, dict):
                 print('macros parameter must be of type dict, not: {}'.format(type(macros)))
             else:
                 for key, val in macros.items():
                     self._shared.add_macro(key, val, action)
-        for arg, val in args.items():
-            sub = SubElement(action, arg)
-            sub.text = str(val)
+        if isScript:
+            script_element = SubElement(action, 'script')
+            script_element.attrib['file'] = args['file']
+            if args.get('script') is not None:
+                text_element = SubElement(script_element, 'text')
+                text_element.text = args['script']
+        else:
+            for arg, val in args.items():
+                sub = SubElement(action, arg)
+                sub.text = str(val)
 
     def action_execute_as_one(self, val: bool) -> None:
         """
         Add execute all actions as one property to widget (execute all actions on button press)
 
         :param val: Execute all actions as one?
         """
@@ -765,64 +772,100 @@
         if target.lower() not in possible_targets:
             print('Target must be one of {}, not: {}'.format(possible_targets, target))
             return
         if macros is not None and not isinstance(macros, dict):
             print('The macro parameter must be a dictionary with key=MacroName and val=MacroValue')
             return
         args = {'file': file, 'target': target.lower()}
-        self._add_action('open_display', description, args, macros)
+        self._add_action('open_display', description, args, False, macros)
 
     def action_write_pv(self, pv_name: str, value: Union[str, int, float], description: str = None) -> None:
         """
         Add Write PV action to widget. description is optional
 
         :param pv_name: PV name to write to
         :param value: Value to write to PV
         :param description: Description of action. Default is None
         """
         if description is None:
             description = 'Write PV'
         args = {'pv_name': pv_name, 'value': value}
-        self._add_action('write_pv', description, args)
+        self._add_action('write_pv', description, args, False)
 
     def action_execute_command(self, command: str, description: str = None) -> None:
         """
         Add Execute Command action to widget. description is optional
 
         :param command: Command to run in action
         :param description: Description of action. Default is None
         """
         if description is None:
             description = 'Execute Command'
         args = {'command': command}
-        self._add_action('command', description, args)
+        self._add_action('command', description, args, False)
+
+    def action_execute_python_script(self, script: str, description: str = None) -> None:
+        """
+        Add Execute Command action to widget. description is optional
+
+        :param script: Python script to execute as action
+        :param description: Description of action. Default is None
+        """
+        if description is None:
+            description = 'Execute Script'
+        args = {'file': 'EmbeddedPy', 'script': script}
+        self._add_action('execute', description, args, True)
+
+    def action_execute_javascript_script(self, script: str, description: str = None) -> None:
+        """
+        Add Execute Command action to widget. description is optional
+
+        :param script: Javascript code to execute as action
+        :param description: Description of action. Default is None
+        """
+        if description is None:
+            description = 'Execute Script'
+        args = {'file': 'EmbeddedJs', 'script': script}
+        self._add_action('execute', description, args, True)
+
+    def action_execute_external_script(self, file_name: str, description: str = None) -> None:
+        """
+        Add Execute Command action to widget. description is optional
+
+        :param file_name: External script file name
+        :param description: Description of action. Default is None
+        """
+        if description is None:
+            description = 'Execute Script'
+        args = {'file': file_name}
+        self._add_action('execute', description, args, True)
 
     def action_open_file(self, file: str, description: str = None) -> None:
         """
         Add Open File action to widget. description is optional
 
         :param file: File name to open
         :param description: Description of action. Default is None
         """
         if description is None:
             description = 'Open File'
         args = {'file': file}
-        self._add_action('open_file', description, args)
+        self._add_action('open_file', description, args, False)
 
     def action_open_webpage(self, url: str, description: str = None) -> None:
         """
         Add Open Webpage action to widget. description is optional
 
         :param url: URL to open
         :param description: Description of action. Default is None
         """
         if description is None:
             description = 'Open Webpage'
         args = {'url': url}
-        self._add_action('open_webpage', description, args)
+        self._add_action('open_webpage', description, args, False)
 
 class _Label(object):
     def label(self, val: str) -> None:
         """
         Add label to widget
 
         :param val: Label
```

### Comparing `phoebusgen-2.6.0/phoebusgen/widget/widget.py` & `phoebusgen-2.6.1/phoebusgen/widget/widget.py`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.6.0/phoebusgen/widget/widgets.py` & `phoebusgen-2.6.1/phoebusgen/widget/widgets.py`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.6.0/phoebusgen.egg-info/PKG-INFO` & `phoebusgen-2.6.1/phoebusgen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phoebusgen
-Version: 2.6.0
+Version: 2.6.1
 Summary: Control screen generator for Phoebus
 Home-page: https://github.com/tynanford/phoebusgen
 Author: Tynan Ford
 Author-email: tford@lbl.gov
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
```

### Comparing `phoebusgen-2.6.0/phoebusgen.egg-info/SOURCES.txt` & `phoebusgen-2.6.1/phoebusgen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.6.0/setup.py` & `phoebusgen-2.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.6.0/tests/test_screen.py` & `phoebusgen-2.6.1/tests/test_screen.py`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.6.0/tests/test_widget.py` & `phoebusgen-2.6.1/tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.6.0/tests/test_widgets.py` & `phoebusgen-2.6.1/tests/test_widgets.py`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.6.0/versioneer.py` & `phoebusgen-2.6.1/versioneer.py`

 * *Files identical despite different names*

