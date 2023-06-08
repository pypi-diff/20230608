# Comparing `tmp/deform_extensions-0.7.tar.gz` & `tmp/deform_extensions-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deform_extensions-0.7.tar", last modified: Thu Jun  8 13:40:02 2023, max compression
+gzip compressed data, was "deform_extensions-0.8.tar", last modified: Thu Jun  8 14:15:30 2023, max compression
```

## Comparing `deform_extensions-0.7.tar` & `deform_extensions-0.8.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-08 13:40:02.012359 deform_extensions-0.7/
--rw-r--r--   0 gas       (1000) gas       (1000)    35147 2020-10-06 10:02:49.000000 deform_extensions-0.7/LICENSE.txt
--rw-r--r--   0 gas       (1000) gas       (1000)       82 2020-10-06 10:02:49.000000 deform_extensions-0.7/MANIFEST.in
--rw-r--r--   0 gas       (1000) gas       (1000)     2404 2023-06-08 13:40:02.013359 deform_extensions-0.7/PKG-INFO
--rw-r--r--   0 gas       (1000) gas       (1000)     1711 2021-12-14 15:06:53.000000 deform_extensions-0.7/README.rst
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-08 13:40:02.005359 deform_extensions-0.7/deform_extensions/
--rw-r--r--   0 gas       (1000) gas       (1000)    26451 2023-06-08 11:55:28.000000 deform_extensions-0.7/deform_extensions/__init__.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-08 13:40:02.008359 deform_extensions-0.7/deform_extensions/__pycache__/
--rw-r--r--   0 gas       (1000) gas       (1000)    24248 2021-10-28 16:04:22.000000 deform_extensions-0.7/deform_extensions/__pycache__/__init__.cpython-37-pytest-6.2.1.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)    25750 2021-10-29 08:54:35.000000 deform_extensions-0.7/deform_extensions/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)    25568 2020-11-04 09:45:43.000000 deform_extensions-0.7/deform_extensions/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)    24940 2023-06-08 13:38:09.000000 deform_extensions-0.7/deform_extensions/__pycache__/__init__.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)    23995 2023-06-07 16:19:47.000000 deform_extensions-0.7/deform_extensions/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     7313 2021-10-28 16:04:23.000000 deform_extensions-0.7/deform_extensions/__pycache__/test_it.cpython-37-pytest-6.2.1.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     6457 2023-06-08 13:38:10.000000 deform_extensions-0.7/deform_extensions/__pycache__/test_it.cpython-39-pytest-6.2.5.pyc
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-08 13:40:02.009359 deform_extensions-0.7/deform_extensions/resources/
--rw-r--r--   0 gas       (1000) gas       (1000)     1349 2020-10-06 10:02:49.000000 deform_extensions-0.7/deform_extensions/resources/checkbox_toggle.js
--rw-r--r--   0 gas       (1000) gas       (1000)     1473 2020-10-06 10:02:49.000000 deform_extensions-0.7/deform_extensions/resources/date.js
--rw-r--r--   0 gas       (1000) gas       (1000)     1591 2020-10-06 10:02:49.000000 deform_extensions-0.7/deform_extensions/resources/radio_choice_toggle.js
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-08 13:40:02.011359 deform_extensions-0.7/deform_extensions/templates/
--rw-r--r--   0 gas       (1000) gas       (1000)     6748 2023-06-08 13:37:34.000000 deform_extensions-0.7/deform_extensions/templates/accordion_form.pt
--rw-r--r--   0 gas       (1000) gas       (1000)     2550 2023-06-08 11:55:28.000000 deform_extensions-0.7/deform_extensions/templates/accordion_mapping.pt
--rw-r--r--   0 gas       (1000) gas       (1000)     2997 2023-06-08 11:55:28.000000 deform_extensions-0.7/deform_extensions/templates/accordions_mapping.pt
--rw-r--r--   0 gas       (1000) gas       (1000)     1094 2020-10-06 10:02:49.000000 deform_extensions-0.7/deform_extensions/templates/checkbox_toggle.pt
--rw-r--r--   0 gas       (1000) gas       (1000)     1827 2020-10-06 10:02:49.000000 deform_extensions-0.7/deform_extensions/templates/chosen_optgroup.pt
--rw-r--r--   0 gas       (1000) gas       (1000)     1398 2020-10-06 10:02:49.000000 deform_extensions-0.7/deform_extensions/templates/datetimeinput.pt
--rw-r--r--   0 gas       (1000) gas       (1000)      110 2020-10-06 10:02:49.000000 deform_extensions-0.7/deform_extensions/templates/disabledinput.pt
--rw-r--r--   0 gas       (1000) gas       (1000)     4096 2020-10-06 10:02:49.000000 deform_extensions-0.7/deform_extensions/templates/grid_form.pt
--rw-r--r--   0 gas       (1000) gas       (1000)      969 2020-10-06 10:02:49.000000 deform_extensions-0.7/deform_extensions/templates/grid_mapping.pt
--rw-r--r--   0 gas       (1000) gas       (1000)     1984 2020-10-06 10:02:49.000000 deform_extensions-0.7/deform_extensions/templates/grid_mapping_item.pt
--rw-r--r--   0 gas       (1000) gas       (1000)      689 2020-10-06 10:02:49.000000 deform_extensions-0.7/deform_extensions/templates/inline_mapping.pt
--rw-r--r--   0 gas       (1000) gas       (1000)     2000 2020-10-06 10:02:49.000000 deform_extensions-0.7/deform_extensions/templates/inline_mapping_item.pt
--rw-r--r--   0 gas       (1000) gas       (1000)     1164 2020-10-06 10:02:49.000000 deform_extensions-0.7/deform_extensions/templates/radio_choice_toggle.pt
--rw-r--r--   0 gas       (1000) gas       (1000)     2944 2020-10-06 10:02:49.000000 deform_extensions-0.7/deform_extensions/test_it.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-08 13:40:02.006359 deform_extensions-0.7/deform_extensions.egg-info/
--rw-r--r--   0 gas       (1000) gas       (1000)     2404 2023-06-08 13:40:01.000000 deform_extensions-0.7/deform_extensions.egg-info/PKG-INFO
--rw-r--r--   0 gas       (1000) gas       (1000)     1687 2023-06-08 13:40:01.000000 deform_extensions-0.7/deform_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 gas       (1000) gas       (1000)        1 2023-06-08 13:40:01.000000 deform_extensions-0.7/deform_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 gas       (1000) gas       (1000)       68 2023-06-08 13:40:01.000000 deform_extensions-0.7/deform_extensions.egg-info/entry_points.txt
--rw-r--r--   0 gas       (1000) gas       (1000)        1 2020-10-06 10:03:15.000000 deform_extensions-0.7/deform_extensions.egg-info/not-zip-safe
--rw-r--r--   0 gas       (1000) gas       (1000)       70 2023-06-08 13:40:01.000000 deform_extensions-0.7/deform_extensions.egg-info/requires.txt
--rw-r--r--   0 gas       (1000) gas       (1000)       18 2023-06-08 13:40:01.000000 deform_extensions-0.7/deform_extensions.egg-info/top_level.txt
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-08 13:40:02.011359 deform_extensions-0.7/docs/
--rw-r--r--   0 gas       (1000) gas       (1000)     6815 2020-10-06 10:02:49.000000 deform_extensions-0.7/docs/Makefile
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-08 13:40:02.012359 deform_extensions-0.7/docs/source/
--rw-r--r--   0 gas       (1000) gas       (1000)     8363 2020-10-06 10:02:49.000000 deform_extensions-0.7/docs/source/conf.py
--rw-r--r--   0 gas       (1000) gas       (1000)      187 2020-10-06 10:02:49.000000 deform_extensions-0.7/docs/source/deform_extensions.rst
--rw-r--r--   0 gas       (1000) gas       (1000)      491 2020-10-06 10:02:49.000000 deform_extensions-0.7/docs/source/index.rst
--rw-r--r--   0 gas       (1000) gas       (1000)       98 2020-10-06 10:02:49.000000 deform_extensions-0.7/docs/source/modules.rst
--rw-r--r--   0 gas       (1000) gas       (1000)      194 2023-06-08 13:40:02.013359 deform_extensions-0.7/setup.cfg
--rw-r--r--   0 gas       (1000) gas       (1000)     1505 2023-06-08 13:39:24.000000 deform_extensions-0.7/setup.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-08 14:15:30.486797 deform_extensions-0.8/
+-rw-r--r--   0 gas       (1000) gas       (1000)    35147 2020-10-06 10:02:49.000000 deform_extensions-0.8/LICENSE.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)       82 2020-10-06 10:02:49.000000 deform_extensions-0.8/MANIFEST.in
+-rw-r--r--   0 gas       (1000) gas       (1000)     2404 2023-06-08 14:15:30.486797 deform_extensions-0.8/PKG-INFO
+-rw-r--r--   0 gas       (1000) gas       (1000)     1711 2021-12-14 15:06:53.000000 deform_extensions-0.8/README.rst
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-08 14:15:30.478797 deform_extensions-0.8/deform_extensions/
+-rw-r--r--   0 gas       (1000) gas       (1000)    26451 2023-06-08 11:55:28.000000 deform_extensions-0.8/deform_extensions/__init__.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-08 14:15:30.482797 deform_extensions-0.8/deform_extensions/__pycache__/
+-rw-r--r--   0 gas       (1000) gas       (1000)    24248 2021-10-28 16:04:22.000000 deform_extensions-0.8/deform_extensions/__pycache__/__init__.cpython-37-pytest-6.2.1.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)    25750 2021-10-29 08:54:35.000000 deform_extensions-0.8/deform_extensions/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)    25568 2020-11-04 09:45:43.000000 deform_extensions-0.8/deform_extensions/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)    24940 2023-06-08 13:38:09.000000 deform_extensions-0.8/deform_extensions/__pycache__/__init__.cpython-39-pytest-6.2.5.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)    23995 2023-06-07 16:19:47.000000 deform_extensions-0.8/deform_extensions/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     7313 2021-10-28 16:04:23.000000 deform_extensions-0.8/deform_extensions/__pycache__/test_it.cpython-37-pytest-6.2.1.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     6457 2023-06-08 13:38:10.000000 deform_extensions-0.8/deform_extensions/__pycache__/test_it.cpython-39-pytest-6.2.5.pyc
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-08 14:15:30.482797 deform_extensions-0.8/deform_extensions/resources/
+-rw-r--r--   0 gas       (1000) gas       (1000)     1349 2020-10-06 10:02:49.000000 deform_extensions-0.8/deform_extensions/resources/checkbox_toggle.js
+-rw-r--r--   0 gas       (1000) gas       (1000)     1473 2020-10-06 10:02:49.000000 deform_extensions-0.8/deform_extensions/resources/date.js
+-rw-r--r--   0 gas       (1000) gas       (1000)     1591 2020-10-06 10:02:49.000000 deform_extensions-0.8/deform_extensions/resources/radio_choice_toggle.js
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-08 14:15:30.485797 deform_extensions-0.8/deform_extensions/templates/
+-rw-r--r--   0 gas       (1000) gas       (1000)     6741 2023-06-08 14:15:05.000000 deform_extensions-0.8/deform_extensions/templates/accordion_form.pt
+-rw-r--r--   0 gas       (1000) gas       (1000)     2550 2023-06-08 11:55:28.000000 deform_extensions-0.8/deform_extensions/templates/accordion_mapping.pt
+-rw-r--r--   0 gas       (1000) gas       (1000)     3341 2023-06-08 14:15:01.000000 deform_extensions-0.8/deform_extensions/templates/accordions_mapping.pt
+-rw-r--r--   0 gas       (1000) gas       (1000)     1094 2020-10-06 10:02:49.000000 deform_extensions-0.8/deform_extensions/templates/checkbox_toggle.pt
+-rw-r--r--   0 gas       (1000) gas       (1000)     1827 2020-10-06 10:02:49.000000 deform_extensions-0.8/deform_extensions/templates/chosen_optgroup.pt
+-rw-r--r--   0 gas       (1000) gas       (1000)     1398 2020-10-06 10:02:49.000000 deform_extensions-0.8/deform_extensions/templates/datetimeinput.pt
+-rw-r--r--   0 gas       (1000) gas       (1000)      110 2020-10-06 10:02:49.000000 deform_extensions-0.8/deform_extensions/templates/disabledinput.pt
+-rw-r--r--   0 gas       (1000) gas       (1000)     4096 2020-10-06 10:02:49.000000 deform_extensions-0.8/deform_extensions/templates/grid_form.pt
+-rw-r--r--   0 gas       (1000) gas       (1000)      969 2020-10-06 10:02:49.000000 deform_extensions-0.8/deform_extensions/templates/grid_mapping.pt
+-rw-r--r--   0 gas       (1000) gas       (1000)     1984 2020-10-06 10:02:49.000000 deform_extensions-0.8/deform_extensions/templates/grid_mapping_item.pt
+-rw-r--r--   0 gas       (1000) gas       (1000)      689 2020-10-06 10:02:49.000000 deform_extensions-0.8/deform_extensions/templates/inline_mapping.pt
+-rw-r--r--   0 gas       (1000) gas       (1000)     2000 2020-10-06 10:02:49.000000 deform_extensions-0.8/deform_extensions/templates/inline_mapping_item.pt
+-rw-r--r--   0 gas       (1000) gas       (1000)     1164 2020-10-06 10:02:49.000000 deform_extensions-0.8/deform_extensions/templates/radio_choice_toggle.pt
+-rw-r--r--   0 gas       (1000) gas       (1000)     2944 2020-10-06 10:02:49.000000 deform_extensions-0.8/deform_extensions/test_it.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-08 14:15:30.479797 deform_extensions-0.8/deform_extensions.egg-info/
+-rw-r--r--   0 gas       (1000) gas       (1000)     2404 2023-06-08 14:15:29.000000 deform_extensions-0.8/deform_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 gas       (1000) gas       (1000)     1687 2023-06-08 14:15:30.000000 deform_extensions-0.8/deform_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)        1 2023-06-08 14:15:30.000000 deform_extensions-0.8/deform_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)       68 2023-06-08 14:15:30.000000 deform_extensions-0.8/deform_extensions.egg-info/entry_points.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)        1 2020-10-06 10:03:15.000000 deform_extensions-0.8/deform_extensions.egg-info/not-zip-safe
+-rw-r--r--   0 gas       (1000) gas       (1000)       70 2023-06-08 14:15:30.000000 deform_extensions-0.8/deform_extensions.egg-info/requires.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)       18 2023-06-08 14:15:30.000000 deform_extensions-0.8/deform_extensions.egg-info/top_level.txt
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-08 14:15:30.485797 deform_extensions-0.8/docs/
+-rw-r--r--   0 gas       (1000) gas       (1000)     6815 2020-10-06 10:02:49.000000 deform_extensions-0.8/docs/Makefile
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-08 14:15:30.486797 deform_extensions-0.8/docs/source/
+-rw-r--r--   0 gas       (1000) gas       (1000)     8363 2020-10-06 10:02:49.000000 deform_extensions-0.8/docs/source/conf.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      187 2020-10-06 10:02:49.000000 deform_extensions-0.8/docs/source/deform_extensions.rst
+-rw-r--r--   0 gas       (1000) gas       (1000)      491 2020-10-06 10:02:49.000000 deform_extensions-0.8/docs/source/index.rst
+-rw-r--r--   0 gas       (1000) gas       (1000)       98 2020-10-06 10:02:49.000000 deform_extensions-0.8/docs/source/modules.rst
+-rw-r--r--   0 gas       (1000) gas       (1000)      194 2023-06-08 14:15:30.486797 deform_extensions-0.8/setup.cfg
+-rw-r--r--   0 gas       (1000) gas       (1000)     1505 2023-06-08 14:13:09.000000 deform_extensions-0.8/setup.py
```

### Comparing `deform_extensions-0.7/LICENSE.txt` & `deform_extensions-0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deform_extensions-0.7/PKG-INFO` & `deform_extensions-0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deform_extensions
-Version: 0.7
+Version: 0.8
 Summary: Usefull tools for making grid/accordion layouted forms
 Home-page: https://github.com/majerteam/deform_extensions
 Author: Gaston Tjebbes - Majerti
 Author-email: tech@majerti.fr
 License: GPLv3
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `deform_extensions-0.7/README.rst` & `deform_extensions-0.8/README.rst`

 * *Files identical despite different names*

### Comparing `deform_extensions-0.7/deform_extensions/__init__.py` & `deform_extensions-0.8/deform_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `deform_extensions-0.7/deform_extensions/__pycache__/__init__.cpython-37-pytest-6.2.1.pyc` & `deform_extensions-0.8/deform_extensions/__pycache__/__init__.cpython-37-pytest-6.2.1.pyc`

 * *Files identical despite different names*

### Comparing `deform_extensions-0.7/deform_extensions/__pycache__/__init__.cpython-37.pyc` & `deform_extensions-0.8/deform_extensions/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `deform_extensions-0.7/deform_extensions/__pycache__/__init__.cpython-38.pyc` & `deform_extensions-0.8/deform_extensions/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deform_extensions-0.7/deform_extensions/__pycache__/__init__.cpython-39-pytest-6.2.5.pyc` & `deform_extensions-0.8/deform_extensions/__pycache__/__init__.cpython-39-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `deform_extensions-0.7/deform_extensions/__pycache__/__init__.cpython-39.pyc` & `deform_extensions-0.8/deform_extensions/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deform_extensions-0.7/deform_extensions/__pycache__/test_it.cpython-37-pytest-6.2.1.pyc` & `deform_extensions-0.8/deform_extensions/__pycache__/test_it.cpython-37-pytest-6.2.1.pyc`

 * *Files identical despite different names*

### Comparing `deform_extensions-0.7/deform_extensions/__pycache__/test_it.cpython-39-pytest-6.2.5.pyc` & `deform_extensions-0.8/deform_extensions/__pycache__/test_it.cpython-39-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `deform_extensions-0.7/deform_extensions/resources/checkbox_toggle.js` & `deform_extensions-0.8/deform_extensions/resources/checkbox_toggle.js`

 * *Files identical despite different names*

### Comparing `deform_extensions-0.7/deform_extensions/resources/date.js` & `deform_extensions-0.8/deform_extensions/resources/date.js`

 * *Files identical despite different names*

### Comparing `deform_extensions-0.7/deform_extensions/resources/radio_choice_toggle.js` & `deform_extensions-0.8/deform_extensions/resources/radio_choice_toggle.js`

 * *Files identical despite different names*

### Comparing `deform_extensions-0.7/deform_extensions/templates/accordion_form.pt` & `deform_extensions-0.8/deform_extensions/templates/accordion_form.pt`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
       <p class="errorMsg">${field.errormsg}</p>
     </div>
 
     <p class="section first" tal:condition="description">
       ${description}
     </p>
 
-    <div tal:omit-tag="" tal:condition="${field.widget.fallback_section=='top'}" tal:repeat="field external_fields">
+    <div tal:omit-tag="" tal:condition="field.widget.fallback_section=='top'" tal:repeat="field external_fields">
       <tal:block tal:omit-tag="" tal:condition="field">
         <div tal:replace="structure field.render_template(default_item_template)" />
       </tal:block>
     </div>
 
     <div class='panel-group' id='form-accordion' role="tablist" aria-multiselectable="true">
 
@@ -106,15 +106,15 @@
                   </tal:block>
                 </div>
             </div>
           </tal:if>
         </div>
       </div>
     </div>
-    <div tal:omit-tag="" tal:condition="${field.widget.fallback_section=='down'}" tal:repeat="field external_fields">
+   <div tal:omit-tag="" tal:condition="field.widget.fallback_section=='down'" tal:repeat="field external_fields">
       <tal:block tal:omit-tag="" tal:condition="field">
         <div tal:replace="structure field.render_template(default_item_template)" />
       </tal:block>
     </div>
 
 
     <!-- Append the buttons at the end -->
```

### Comparing `deform_extensions-0.7/deform_extensions/templates/accordion_mapping.pt` & `deform_extensions-0.8/deform_extensions/templates/accordion_mapping.pt`

 * *Files identical despite different names*

### Comparing `deform_extensions-0.7/deform_extensions/templates/accordions_mapping.pt` & `deform_extensions-0.8/deform_extensions/templates/accordions_mapping.pt`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 				fields python: field.widget.accordions(field);
 				external_fields fields[0];
 				accordions fields[1];
 				grid_item_template item_template|field.widget.item_template;
 				default_item_template default_item_template|field.widget.default_item_template;
 				"
 	>
-		<div tal:omit-tag="" tal:repeat="field top_level_fields">
+        <div tal:omit-tag="" tal:condition="field.widget.fallback_section=='top'" tal:repeat="field external_fields">
 			<tal:block tal:omit-tag="" tal:condition="field">
 				<div tal:replace="structure field.render_template(default_item_template)" />
 			</tal:block>
 		</div>
 
 		<div class='collapsible' id='mapping-${field.widget.tag_id}-accordion' role="tablist" aria-multiselectable="true">
 			<div class="separate_block border_left_block"
@@ -73,8 +73,13 @@
 									</div>
 							</div>
 						</tal:if>
 					</div>
 				</div>
 			</div>
 		</div>
+    <div tal:omit-tag="" tal:condition="field.widget.fallback_section=='down'" tal:repeat="field external_fields">
+      <tal:block tal:omit-tag="" tal:condition="field">
+        <div tal:replace="structure field.render_template(default_item_template)" />
+      </tal:block>
+    </div>
 </tal:custom>
```

### Comparing `deform_extensions-0.7/deform_extensions/templates/checkbox_toggle.pt` & `deform_extensions-0.8/deform_extensions/templates/checkbox_toggle.pt`

 * *Files identical despite different names*

### Comparing `deform_extensions-0.7/deform_extensions/templates/chosen_optgroup.pt` & `deform_extensions-0.8/deform_extensions/templates/chosen_optgroup.pt`

 * *Files identical despite different names*

### Comparing `deform_extensions-0.7/deform_extensions/templates/datetimeinput.pt` & `deform_extensions-0.8/deform_extensions/templates/datetimeinput.pt`

 * *Files identical despite different names*

### Comparing `deform_extensions-0.7/deform_extensions/templates/grid_form.pt` & `deform_extensions-0.8/deform_extensions/templates/grid_form.pt`

 * *Files identical despite different names*

### Comparing `deform_extensions-0.7/deform_extensions/templates/grid_mapping.pt` & `deform_extensions-0.8/deform_extensions/templates/grid_mapping.pt`

 * *Files identical despite different names*

### Comparing `deform_extensions-0.7/deform_extensions/templates/grid_mapping_item.pt` & `deform_extensions-0.8/deform_extensions/templates/grid_mapping_item.pt`

 * *Files identical despite different names*

### Comparing `deform_extensions-0.7/deform_extensions/templates/inline_mapping.pt` & `deform_extensions-0.8/deform_extensions/templates/inline_mapping.pt`

 * *Files identical despite different names*

### Comparing `deform_extensions-0.7/deform_extensions/templates/inline_mapping_item.pt` & `deform_extensions-0.8/deform_extensions/templates/inline_mapping_item.pt`

 * *Files identical despite different names*

### Comparing `deform_extensions-0.7/deform_extensions/templates/radio_choice_toggle.pt` & `deform_extensions-0.8/deform_extensions/templates/radio_choice_toggle.pt`

 * *Files identical despite different names*

### Comparing `deform_extensions-0.7/deform_extensions/test_it.py` & `deform_extensions-0.8/deform_extensions/test_it.py`

 * *Files identical despite different names*

### Comparing `deform_extensions-0.7/deform_extensions.egg-info/PKG-INFO` & `deform_extensions-0.8/deform_extensions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deform-extensions
-Version: 0.7
+Version: 0.8
 Summary: Usefull tools for making grid/accordion layouted forms
 Home-page: https://github.com/majerteam/deform_extensions
 Author: Gaston Tjebbes - Majerti
 Author-email: tech@majerti.fr
 License: GPLv3
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `deform_extensions-0.7/deform_extensions.egg-info/SOURCES.txt` & `deform_extensions-0.8/deform_extensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deform_extensions-0.7/docs/Makefile` & `deform_extensions-0.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `deform_extensions-0.7/docs/source/conf.py` & `deform_extensions-0.8/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `deform_extensions-0.7/setup.py` & `deform_extensions-0.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='deform_extensions',
-    version='0.7',
+    version='0.8',
     packages=['deform_extensions'],
     include_package_data=True,
     license='GPLv3',
     description='Usefull tools for making grid/accordion layouted forms',
     long_description=README,
     url='https://github.com/majerteam/deform_extensions',
     author='Gaston Tjebbes - Majerti',
```

