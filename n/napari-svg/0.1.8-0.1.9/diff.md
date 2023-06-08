# Comparing `tmp/napari-svg-0.1.8.tar.gz` & `tmp/napari-svg-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-svg-0.1.8.tar", last modified: Mon Jun  5 13:01:17 2023, max compression
+gzip compressed data, was "napari-svg-0.1.9.tar", last modified: Thu Jun  8 15:39:12 2023, max compression
```

## Comparing `napari-svg-0.1.8.tar` & `napari-svg-0.1.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:01:17.290155 napari-svg-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-05 13:01:07.000000 napari-svg-0.1.8/.cruft.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:01:17.286155 napari-svg-0.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:01:17.286155 napari-svg-0.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-06-05 13:01:07.000000 napari-svg-0.1.8/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-05 13:01:07.000000 napari-svg-0.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-05 13:01:07.000000 napari-svg-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-05 13:01:07.000000 napari-svg-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-06-05 13:01:17.290155 napari-svg-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-05 13:01:07.000000 napari-svg-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:01:17.286155 napari-svg-0.1.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-05 13:01:07.000000 napari-svg-0.1.8/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-05 13:01:07.000000 napari-svg-0.1.8/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:01:17.286155 napari-svg-0.1.8/napari_svg/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-05 13:01:07.000000 napari-svg-0.1.8/napari_svg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-06-05 13:01:07.000000 napari-svg-0.1.8/napari_svg/_shape_to_xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:01:17.290155 napari-svg-0.1.8/napari_svg/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 13:01:07.000000 napari-svg-0.1.8/napari_svg/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-05 13:01:07.000000 napari-svg-0.1.8/napari_svg/_tests/test_get_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-06-05 13:01:07.000000 napari-svg-0.1.8/napari_svg/_tests/test_write_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-05 13:01:17.000000 napari-svg-0.1.8/napari_svg/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9253 2023-06-05 13:01:07.000000 napari-svg-0.1.8/napari_svg/hook_implementations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10219 2023-06-05 13:01:07.000000 napari-svg-0.1.8/napari_svg/layer_to_xml.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-05 13:01:07.000000 napari-svg-0.1.8/napari_svg/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-05 13:01:07.000000 napari-svg-0.1.8/napari_svg/xml_to_svg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:01:17.290155 napari-svg-0.1.8/napari_svg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-06-05 13:01:17.000000 napari-svg-0.1.8/napari_svg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-05 13:01:17.000000 napari-svg-0.1.8/napari_svg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 13:01:17.000000 napari-svg-0.1.8/napari_svg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-05 13:01:17.000000 napari-svg-0.1.8/napari_svg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 13:01:17.000000 napari-svg-0.1.8/napari_svg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-05 13:01:17.000000 napari-svg-0.1.8/napari_svg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-05 13:01:17.000000 napari-svg-0.1.8/napari_svg.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:01:17.290155 napari-svg-0.1.8/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-05 13:01:07.000000 napari-svg-0.1.8/requirements/default.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-05 13:01:07.000000 napari-svg-0.1.8/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-05 13:01:07.000000 napari-svg-0.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-05 13:01:17.290155 napari-svg-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-05 13:01:07.000000 napari-svg-0.1.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-05 13:01:07.000000 napari-svg-0.1.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:39:12.541046 napari-svg-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-08 15:39:00.000000 napari-svg-0.1.9/.cruft.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:39:12.537046 napari-svg-0.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:39:12.537046 napari-svg-0.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-06-08 15:39:00.000000 napari-svg-0.1.9/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-08 15:39:00.000000 napari-svg-0.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-08 15:39:00.000000 napari-svg-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-08 15:39:00.000000 napari-svg-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-06-08 15:39:12.541046 napari-svg-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-08 15:39:00.000000 napari-svg-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:39:12.537046 napari-svg-0.1.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-08 15:39:00.000000 napari-svg-0.1.9/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-08 15:39:00.000000 napari-svg-0.1.9/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:39:12.541046 napari-svg-0.1.9/napari_svg/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-08 15:39:00.000000 napari-svg-0.1.9/napari_svg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-06-08 15:39:00.000000 napari-svg-0.1.9/napari_svg/_shape_to_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:39:12.541046 napari-svg-0.1.9/napari_svg/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:39:00.000000 napari-svg-0.1.9/napari_svg/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-08 15:39:00.000000 napari-svg-0.1.9/napari_svg/_tests/test_get_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-06-08 15:39:00.000000 napari-svg-0.1.9/napari_svg/_tests/test_write_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-08 15:39:12.000000 napari-svg-0.1.9/napari_svg/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9253 2023-06-08 15:39:00.000000 napari-svg-0.1.9/napari_svg/hook_implementations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10219 2023-06-08 15:39:00.000000 napari-svg-0.1.9/napari_svg/layer_to_xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-08 15:39:00.000000 napari-svg-0.1.9/napari_svg/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-08 15:39:00.000000 napari-svg-0.1.9/napari_svg/xml_to_svg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:39:12.541046 napari-svg-0.1.9/napari_svg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-06-08 15:39:12.000000 napari-svg-0.1.9/napari_svg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-08 15:39:12.000000 napari-svg-0.1.9/napari_svg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 15:39:12.000000 napari-svg-0.1.9/napari_svg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-08 15:39:12.000000 napari-svg-0.1.9/napari_svg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 15:39:12.000000 napari-svg-0.1.9/napari_svg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-08 15:39:12.000000 napari-svg-0.1.9/napari_svg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-08 15:39:12.000000 napari-svg-0.1.9/napari_svg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:39:12.541046 napari-svg-0.1.9/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-08 15:39:00.000000 napari-svg-0.1.9/requirements/default.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-08 15:39:00.000000 napari-svg-0.1.9/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-08 15:39:00.000000 napari-svg-0.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-08 15:39:12.541046 napari-svg-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-08 15:39:00.000000 napari-svg-0.1.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-08 15:39:00.000000 napari-svg-0.1.9/tox.ini
```

### Comparing `napari-svg-0.1.8/.cruft.json` & `napari-svg-0.1.9/.cruft.json`

 * *Files identical despite different names*

### Comparing `napari-svg-0.1.8/.github/workflows/test_and_deploy.yml` & `napari-svg-0.1.9/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari-svg-0.1.8/.gitignore` & `napari-svg-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `napari-svg-0.1.8/LICENSE` & `napari-svg-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-svg-0.1.8/PKG-INFO` & `napari-svg-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-svg
-Version: 0.1.8
+Version: 0.1.9
 Summary: A plugin for reading and writing svg files with napari
 Home-page: https://github.com/napari/napari-svg
 Download-URL: https://github.com/napari/napari-svg
 Author: Nicholas Sofroniew
 Author-email: sofroniewn@gmail.com
 License: BSD-3
 Classifier: Development Status :: 4 - Beta
```

### Comparing `napari-svg-0.1.8/README.md` & `napari-svg-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `napari-svg-0.1.8/napari_svg/_shape_to_xml.py` & `napari-svg-0.1.9/napari_svg/_shape_to_xml.py`

 * *Files identical despite different names*

### Comparing `napari-svg-0.1.8/napari_svg/_tests/test_get_writer.py` & `napari-svg-0.1.9/napari_svg/_tests/test_get_writer.py`

 * *Files identical despite different names*

### Comparing `napari-svg-0.1.8/napari_svg/_tests/test_write_layer.py` & `napari-svg-0.1.9/napari_svg/_tests/test_write_layer.py`

 * *Files identical despite different names*

### Comparing `napari-svg-0.1.8/napari_svg/hook_implementations.py` & `napari-svg-0.1.9/napari_svg/hook_implementations.py`

 * *Files identical despite different names*

### Comparing `napari-svg-0.1.8/napari_svg/layer_to_xml.py` & `napari-svg-0.1.9/napari_svg/layer_to_xml.py`

 * *Files identical despite different names*

### Comparing `napari-svg-0.1.8/napari_svg/xml_to_svg.py` & `napari-svg-0.1.9/napari_svg/xml_to_svg.py`

 * *Files identical despite different names*

### Comparing `napari-svg-0.1.8/napari_svg.egg-info/PKG-INFO` & `napari-svg-0.1.9/napari_svg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-svg
-Version: 0.1.8
+Version: 0.1.9
 Summary: A plugin for reading and writing svg files with napari
 Home-page: https://github.com/napari/napari-svg
 Download-URL: https://github.com/napari/napari-svg
 Author: Nicholas Sofroniew
 Author-email: sofroniewn@gmail.com
 License: BSD-3
 Classifier: Development Status :: 4 - Beta
```

### Comparing `napari-svg-0.1.8/napari_svg.egg-info/SOURCES.txt` & `napari-svg-0.1.9/napari_svg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari-svg-0.1.8/setup.cfg` & `napari-svg-0.1.9/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 zip_safe = False
 packages = find:
 python_requires = >=3.7
 install_requires = 
 	imageio>=2.5.0
 	numpy>=1.16.0
 	napari-plugin-engine>=0.1.4
-	vispy>=0.6.4
+	napari>=0.4.0
 
 [options.extras_require]
 testing = 
 	pytest
 	pytest-cov
 	napari >= 0.4
 	pyqt5
```

### Comparing `napari-svg-0.1.8/tox.ini` & `napari-svg-0.1.9/tox.ini`

 * *Files identical despite different names*

