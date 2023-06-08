# Comparing `tmp/html-xblock-1.3.3.tar.gz` & `tmp/html-xblock-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "html-xblock-1.3.3.tar", last modified: Mon Mar  6 13:53:44 2023, max compression
+gzip compressed data, was "html-xblock-1.3.4.tar", last modified: Thu Jun  8 20:13:49 2023, max compression
```

## Comparing `html-xblock-1.3.3.tar` & `html-xblock-1.3.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 13:53:44.547446 html-xblock-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (122)    35136 2023-03-06 13:53:41.000000 html-xblock-1.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-03-06 13:53:41.000000 html-xblock-1.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2730 2023-03-06 13:53:44.543446 html-xblock-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2393 2023-03-06 13:53:41.000000 html-xblock-1.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 13:53:44.543446 html-xblock-1.3.3/html_xblock/
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-03-06 13:53:41.000000 html-xblock-1.3.3/html_xblock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8753 2023-03-06 13:53:41.000000 html-xblock-1.3.3/html_xblock/bleaching.py
--rw-r--r--   0 runner    (1001) docker     (122)    11179 2023-03-06 13:53:41.000000 html-xblock-1.3.3/html_xblock/html.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 13:53:44.539446 html-xblock-1.3.3/html_xblock/public/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 13:53:44.539446 html-xblock-1.3.3/html_xblock/public/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 13:53:44.543446 html-xblock-1.3.3/html_xblock/public/plugins/codesample/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 13:53:44.543446 html-xblock-1.3.3/html_xblock/public/plugins/codesample/css/
--rw-r--r--   0 runner    (1001) docker     (122)     2400 2023-03-06 13:53:41.000000 html-xblock-1.3.3/html_xblock/public/plugins/codesample/css/prism.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 13:53:44.543446 html-xblock-1.3.3/html_xblock/public/plugins/codesample/js/
--rw-r--r--   0 runner    (1001) docker     (122)    23415 2023-03-06 13:53:41.000000 html-xblock-1.3.3/html_xblock/public/plugins/codesample/js/prism.js
--rw-r--r--   0 runner    (1001) docker     (122)    19335 2023-03-06 13:53:41.000000 html-xblock-1.3.3/html_xblock/public/plugins/codesample/plugin.min.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 13:53:44.539446 html-xblock-1.3.3/html_xblock/static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 13:53:44.543446 html-xblock-1.3.3/html_xblock/static/css/
--rw-r--r--   0 runner    (1001) docker     (122)      737 2023-03-06 13:53:41.000000 html-xblock-1.3.3/html_xblock/static/css/html_edit.css
--rw-r--r--   0 runner    (1001) docker     (122)     2332 2023-03-06 13:53:41.000000 html-xblock-1.3.3/html_xblock/static/css/html_preview.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 13:53:44.543446 html-xblock-1.3.3/html_xblock/static/html/
--rw-r--r--   0 runner    (1001) docker     (122)       89 2023-03-06 13:53:41.000000 html-xblock-1.3.3/html_xblock/static/html/lms.html
--rw-r--r--   0 runner    (1001) docker     (122)      992 2023-03-06 13:53:41.000000 html-xblock-1.3.3/html_xblock/static/html/studio.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 13:53:44.543446 html-xblock-1.3.3/html_xblock/static/js/
--rw-r--r--   0 runner    (1001) docker     (122)    10237 2023-03-06 13:53:41.000000 html-xblock-1.3.3/html_xblock/static/js/html_edit.js
--rw-r--r--   0 runner    (1001) docker     (122)      161 2023-03-06 13:53:41.000000 html-xblock-1.3.3/html_xblock/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 13:53:44.543446 html-xblock-1.3.3/html_xblock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2730 2023-03-06 13:53:44.000000 html-xblock-1.3.3/html_xblock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      746 2023-03-06 13:53:44.000000 html-xblock-1.3.3/html_xblock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-06 13:53:44.000000 html-xblock-1.3.3/html_xblock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       93 2023-03-06 13:53:44.000000 html-xblock-1.3.3/html_xblock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-03-06 13:53:44.000000 html-xblock-1.3.3/html_xblock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-03-06 13:53:44.000000 html-xblock-1.3.3/html_xblock.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 13:53:44.543446 html-xblock-1.3.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-03-06 13:53:41.000000 html-xblock-1.3.3/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-03-06 13:53:41.000000 html-xblock-1.3.3/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-06 13:53:44.547446 html-xblock-1.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5031 2023-03-06 13:53:41.000000 html-xblock-1.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 13:53:44.543446 html-xblock-1.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     5335 2023-03-06 13:53:41.000000 html-xblock-1.3.3/tests/test_basics.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 20:13:49.783015 html-xblock-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (122)    35136 2023-06-08 20:13:45.000000 html-xblock-1.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-06-08 20:13:45.000000 html-xblock-1.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2730 2023-06-08 20:13:49.783015 html-xblock-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2393 2023-06-08 20:13:45.000000 html-xblock-1.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 20:13:49.779015 html-xblock-1.3.4/html_xblock/
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-06-08 20:13:45.000000 html-xblock-1.3.4/html_xblock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8774 2023-06-08 20:13:45.000000 html-xblock-1.3.4/html_xblock/bleaching.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11179 2023-06-08 20:13:45.000000 html-xblock-1.3.4/html_xblock/html.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 20:13:49.779015 html-xblock-1.3.4/html_xblock/public/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 20:13:49.779015 html-xblock-1.3.4/html_xblock/public/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 20:13:49.779015 html-xblock-1.3.4/html_xblock/public/plugins/codesample/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 20:13:49.783015 html-xblock-1.3.4/html_xblock/public/plugins/codesample/css/
+-rw-r--r--   0 runner    (1001) docker     (122)     2400 2023-06-08 20:13:45.000000 html-xblock-1.3.4/html_xblock/public/plugins/codesample/css/prism.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 20:13:49.783015 html-xblock-1.3.4/html_xblock/public/plugins/codesample/js/
+-rw-r--r--   0 runner    (1001) docker     (122)    23415 2023-06-08 20:13:45.000000 html-xblock-1.3.4/html_xblock/public/plugins/codesample/js/prism.js
+-rw-r--r--   0 runner    (1001) docker     (122)    19335 2023-06-08 20:13:45.000000 html-xblock-1.3.4/html_xblock/public/plugins/codesample/plugin.min.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 20:13:49.779015 html-xblock-1.3.4/html_xblock/static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 20:13:49.783015 html-xblock-1.3.4/html_xblock/static/css/
+-rw-r--r--   0 runner    (1001) docker     (122)      737 2023-06-08 20:13:45.000000 html-xblock-1.3.4/html_xblock/static/css/html_edit.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2332 2023-06-08 20:13:45.000000 html-xblock-1.3.4/html_xblock/static/css/html_preview.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 20:13:49.783015 html-xblock-1.3.4/html_xblock/static/html/
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-06-08 20:13:45.000000 html-xblock-1.3.4/html_xblock/static/html/lms.html
+-rw-r--r--   0 runner    (1001) docker     (122)      992 2023-06-08 20:13:45.000000 html-xblock-1.3.4/html_xblock/static/html/studio.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 20:13:49.783015 html-xblock-1.3.4/html_xblock/static/js/
+-rw-r--r--   0 runner    (1001) docker     (122)    10237 2023-06-08 20:13:45.000000 html-xblock-1.3.4/html_xblock/static/js/html_edit.js
+-rw-r--r--   0 runner    (1001) docker     (122)      161 2023-06-08 20:13:45.000000 html-xblock-1.3.4/html_xblock/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 20:13:49.779015 html-xblock-1.3.4/html_xblock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2730 2023-06-08 20:13:49.000000 html-xblock-1.3.4/html_xblock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      746 2023-06-08 20:13:49.000000 html-xblock-1.3.4/html_xblock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-08 20:13:49.000000 html-xblock-1.3.4/html_xblock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-06-08 20:13:49.000000 html-xblock-1.3.4/html_xblock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-06-08 20:13:49.000000 html-xblock-1.3.4/html_xblock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-08 20:13:49.000000 html-xblock-1.3.4/html_xblock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 20:13:49.783015 html-xblock-1.3.4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-06-08 20:13:45.000000 html-xblock-1.3.4/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-06-08 20:13:45.000000 html-xblock-1.3.4/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-08 20:13:49.783015 html-xblock-1.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5031 2023-06-08 20:13:45.000000 html-xblock-1.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 20:13:49.783015 html-xblock-1.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     5335 2023-06-08 20:13:45.000000 html-xblock-1.3.4/tests/test_basics.py
```

### Comparing `html-xblock-1.3.3/LICENSE` & `html-xblock-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `html-xblock-1.3.3/PKG-INFO` & `html-xblock-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html-xblock
-Version: 1.3.3
+Version: 1.3.4
 Summary: HTML XBlock will help creating and using a secure and easy-to-use HTML blocks
 Home-page: https://github.com/open-craft/xblock-html
 Author: OpenCraft
 License: AGPL v3
 Keywords: Python edx
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `html-xblock-1.3.3/README.md` & `html-xblock-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `html-xblock-1.3.3/html_xblock/bleaching.py` & `html-xblock-1.3.4/html_xblock/bleaching.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,14 +74,15 @@
             'tbody',
             'td',
             'tfoot',
             'th',
             'thead',
             'tr',
             'u',
+            'style',
             'iframe',
         }
 
         if self.allow_javascript:
             tags |= {'script'}
 
         return tags
```

### Comparing `html-xblock-1.3.3/html_xblock/html.py` & `html-xblock-1.3.4/html_xblock/html.py`

 * *Files identical despite different names*

### Comparing `html-xblock-1.3.3/html_xblock/public/plugins/codesample/css/prism.css` & `html-xblock-1.3.4/html_xblock/public/plugins/codesample/css/prism.css`

 * *Files identical despite different names*

### Comparing `html-xblock-1.3.3/html_xblock/public/plugins/codesample/js/prism.js` & `html-xblock-1.3.4/html_xblock/public/plugins/codesample/js/prism.js`

 * *Files identical despite different names*

### Comparing `html-xblock-1.3.3/html_xblock/public/plugins/codesample/plugin.min.js` & `html-xblock-1.3.4/html_xblock/public/plugins/codesample/plugin.min.js`

 * *Files identical despite different names*

### Comparing `html-xblock-1.3.3/html_xblock/static/css/html_edit.css` & `html-xblock-1.3.4/html_xblock/static/css/html_edit.css`

 * *Files identical despite different names*

### Comparing `html-xblock-1.3.3/html_xblock/static/css/html_preview.css` & `html-xblock-1.3.4/html_xblock/static/css/html_preview.css`

 * *Files identical despite different names*

### Comparing `html-xblock-1.3.3/html_xblock/static/html/studio.html` & `html-xblock-1.3.4/html_xblock/static/html/studio.html`

 * *Files identical despite different names*

### Comparing `html-xblock-1.3.3/html_xblock/static/js/html_edit.js` & `html-xblock-1.3.4/html_xblock/static/js/html_edit.js`

 * *Files identical despite different names*

### Comparing `html-xblock-1.3.3/html_xblock.egg-info/PKG-INFO` & `html-xblock-1.3.4/html_xblock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html-xblock
-Version: 1.3.3
+Version: 1.3.4
 Summary: HTML XBlock will help creating and using a secure and easy-to-use HTML blocks
 Home-page: https://github.com/open-craft/xblock-html
 Author: OpenCraft
 License: AGPL v3
 Keywords: Python edx
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `html-xblock-1.3.3/html_xblock.egg-info/SOURCES.txt` & `html-xblock-1.3.4/html_xblock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `html-xblock-1.3.3/requirements/constraints.txt` & `html-xblock-1.3.4/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `html-xblock-1.3.3/setup.py` & `html-xblock-1.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `html-xblock-1.3.3/tests/test_basics.py` & `html-xblock-1.3.4/tests/test_basics.py`

 * *Files identical despite different names*

