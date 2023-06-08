# Comparing `tmp/circuitpython-kx132-0.1.0.tar.gz` & `tmp/circuitpython-kx132-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-kx132-0.1.0.tar", last modified: Wed Jun  7 16:00:13 2023, max compression
+gzip compressed data, was "circuitpython-kx132-0.2.0.tar", last modified: Thu Jun  8 17:17:54 2023, max compression
```

## Comparing `circuitpython-kx132-0.1.0.tar` & `circuitpython-kx132-0.2.0.tar`

### file list

```diff
@@ -1,40 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:00:13.090606 circuitpython-kx132-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:00:13.082606 circuitpython-kx132-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:00:13.086606 circuitpython-kx132-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-06-07 15:59:57.000000 circuitpython-kx132-0.1.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-07 15:59:57.000000 circuitpython-kx132-0.1.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-07 15:59:57.000000 circuitpython-kx132-0.1.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-07 15:59:57.000000 circuitpython-kx132-0.1.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-07 15:59:57.000000 circuitpython-kx132-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-07 15:59:57.000000 circuitpython-kx132-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13033 2023-06-07 15:59:57.000000 circuitpython-kx132-0.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-07 15:59:57.000000 circuitpython-kx132-0.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-07 15:59:57.000000 circuitpython-kx132-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-06-07 16:00:13.086606 circuitpython-kx132-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-06-07 15:59:57.000000 circuitpython-kx132-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:00:13.086606 circuitpython-kx132-0.1.0/circuitpython_kx132.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-06-07 16:00:13.000000 circuitpython-kx132-0.1.0/circuitpython_kx132.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-07 16:00:13.000000 circuitpython-kx132-0.1.0/circuitpython_kx132.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 16:00:13.000000 circuitpython-kx132-0.1.0/circuitpython_kx132.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-07 16:00:13.000000 circuitpython-kx132-0.1.0/circuitpython_kx132.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-07 16:00:13.000000 circuitpython-kx132-0.1.0/circuitpython_kx132.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:00:13.086606 circuitpython-kx132-0.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:00:13.086606 circuitpython-kx132-0.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-07 15:59:57.000000 circuitpython-kx132-0.1.0/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-07 15:59:57.000000 circuitpython-kx132-0.1.0/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-07 15:59:57.000000 circuitpython-kx132-0.1.0/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-07 15:59:57.000000 circuitpython-kx132-0.1.0/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-07 15:59:57.000000 circuitpython-kx132-0.1.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-07 15:59:57.000000 circuitpython-kx132-0.1.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-07 15:59:57.000000 circuitpython-kx132-0.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-06-07 15:59:57.000000 circuitpython-kx132-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-07 15:59:57.000000 circuitpython-kx132-0.1.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-07 15:59:57.000000 circuitpython-kx132-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-07 15:59:57.000000 circuitpython-kx132-0.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:00:13.086606 circuitpython-kx132-0.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-07 16:00:05.000000 circuitpython-kx132-0.1.0/examples/kx132_acc_range.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-07 16:00:05.000000 circuitpython-kx132-0.1.0/examples/kx132_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-06-07 16:00:05.000000 circuitpython-kx132-0.1.0/kx132.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-07 16:00:05.000000 circuitpython-kx132-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-07 15:59:57.000000 circuitpython-kx132-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 16:00:13.090606 circuitpython-kx132-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:17:54.967893 circuitpython-kx132-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:17:54.963894 circuitpython-kx132-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:17:54.967893 circuitpython-kx132-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-06-08 17:17:40.000000 circuitpython-kx132-0.2.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-08 17:17:40.000000 circuitpython-kx132-0.2.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-08 17:17:40.000000 circuitpython-kx132-0.2.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-08 17:17:40.000000 circuitpython-kx132-0.2.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-08 17:17:40.000000 circuitpython-kx132-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-08 17:17:40.000000 circuitpython-kx132-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13033 2023-06-08 17:17:40.000000 circuitpython-kx132-0.2.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-08 17:17:40.000000 circuitpython-kx132-0.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-08 17:17:40.000000 circuitpython-kx132-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-06-08 17:17:54.967893 circuitpython-kx132-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-06-08 17:17:40.000000 circuitpython-kx132-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:17:54.967893 circuitpython-kx132-0.2.0/circuitpython_kx132.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-06-08 17:17:54.000000 circuitpython-kx132-0.2.0/circuitpython_kx132.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-08 17:17:54.000000 circuitpython-kx132-0.2.0/circuitpython_kx132.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 17:17:54.000000 circuitpython-kx132-0.2.0/circuitpython_kx132.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-08 17:17:54.000000 circuitpython-kx132-0.2.0/circuitpython_kx132.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-08 17:17:54.000000 circuitpython-kx132-0.2.0/circuitpython_kx132.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:17:54.967893 circuitpython-kx132-0.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:17:54.967893 circuitpython-kx132-0.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-08 17:17:40.000000 circuitpython-kx132-0.2.0/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-08 17:17:40.000000 circuitpython-kx132-0.2.0/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-08 17:17:40.000000 circuitpython-kx132-0.2.0/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-08 17:17:40.000000 circuitpython-kx132-0.2.0/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-08 17:17:40.000000 circuitpython-kx132-0.2.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-08 17:17:40.000000 circuitpython-kx132-0.2.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-08 17:17:40.000000 circuitpython-kx132-0.2.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-06-08 17:17:40.000000 circuitpython-kx132-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-08 17:17:40.000000 circuitpython-kx132-0.2.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-08 17:17:40.000000 circuitpython-kx132-0.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-08 17:17:40.000000 circuitpython-kx132-0.2.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:17:54.967893 circuitpython-kx132-0.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-08 17:17:47.000000 circuitpython-kx132-0.2.0/examples/kx132_acc_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-08 17:17:47.000000 circuitpython-kx132-0.2.0/examples/kx132_adp_enabled.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-08 17:17:47.000000 circuitpython-kx132-0.2.0/examples/kx132_output_data_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-08 17:17:47.000000 circuitpython-kx132-0.2.0/examples/kx132_previous_tilt_position_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-08 17:17:47.000000 circuitpython-kx132-0.2.0/examples/kx132_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-08 17:17:47.000000 circuitpython-kx132-0.2.0/examples/kx132_tap_doubletap_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-08 17:17:47.000000 circuitpython-kx132-0.2.0/examples/kx132_tilt_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13842 2023-06-08 17:17:47.000000 circuitpython-kx132-0.2.0/kx132.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-08 17:17:47.000000 circuitpython-kx132-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-08 17:17:40.000000 circuitpython-kx132-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 17:17:54.967893 circuitpython-kx132-0.2.0/setup.cfg
```

### Comparing `circuitpython-kx132-0.1.0/.github/workflows/build.yml` & `circuitpython-kx132-0.2.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-kx132-0.1.0/.github/workflows/release_gh.yml` & `circuitpython-kx132-0.2.0/.github/workflows/release_gh.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-kx132-0.1.0/.gitignore` & `circuitpython-kx132-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `circuitpython-kx132-0.1.0/.pre-commit-config.yaml` & `circuitpython-kx132-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython-kx132-0.1.0/.pylintrc` & `circuitpython-kx132-0.2.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-kx132-0.1.0/LICENSE` & `circuitpython-kx132-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-kx132-0.1.0/PKG-INFO` & `circuitpython-kx132-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-kx132
-Version: 0.1.0
+Version: 0.2.0
 Summary: CircuitPython Driver for the Kionix KX132 Accelerometer
 Author-email: JDM <xxx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_KX132
 Keywords: sensor,blinka,circuitpython,micropython,kx132,acceleration,gravity,accelerometer,sensor,driver,KX132
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-kx132-0.1.0/README.rst` & `circuitpython-kx132-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-kx132-0.1.0/circuitpython_kx132.egg-info/PKG-INFO` & `circuitpython-kx132-0.2.0/circuitpython_kx132.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-kx132
-Version: 0.1.0
+Version: 0.2.0
 Summary: CircuitPython Driver for the Kionix KX132 Accelerometer
 Author-email: JDM <xxx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_KX132
 Keywords: sensor,blinka,circuitpython,micropython,kx132,acceleration,gravity,accelerometer,sensor,driver,KX132
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-kx132-0.1.0/docs/_static/Logo.png` & `circuitpython-kx132-0.2.0/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `circuitpython-kx132-0.1.0/docs/_static/favicon.ico` & `circuitpython-kx132-0.2.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-kx132-0.1.0/docs/conf.py` & `circuitpython-kx132-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circuitpython-kx132-0.1.0/examples/kx132_acc_range.py` & `circuitpython-kx132-0.2.0/examples/kx132_acc_range.py`

 * *Files identical despite different names*

### Comparing `circuitpython-kx132-0.1.0/pyproject.toml` & `circuitpython-kx132-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-kx132"
 description = "CircuitPython Driver for the Kionix KX132 Accelerometer"
-version = "0.1.0"
+version = "0.2.0"
 readme = "README.rst"
 authors = [
     {name = "JDM", email = "xxx@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/CircuitPython_KX132"}
 keywords = [
     "sensor",
```

