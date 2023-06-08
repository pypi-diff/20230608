# Comparing `tmp/pdm-pip-index-url-0.1.0.tar.gz` & `tmp/pdm-pip-index-url-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm-pip-index-url-0.1.0.tar", last modified: Thu Jun  8 11:02:51 2023, max compression
+gzip compressed data, was "pdm-pip-index-url-0.1.1.tar", last modified: Thu Jun  8 11:14:08 2023, max compression
```

## Comparing `pdm-pip-index-url-0.1.0.tar` & `pdm-pip-index-url-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 11:02:51.395123 pdm-pip-index-url-0.1.0/
--rw-rw-rw-   0        0        0      946 2023-06-08 11:02:51.391143 pdm-pip-index-url-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      603 2023-06-08 10:46:57.000000 pdm-pip-index-url-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 11:02:51.370903 pdm-pip-index-url-0.1.0/pdm_pip_index_url/
--rw-rw-rw-   0        0        0      201 2023-06-08 10:44:02.000000 pdm-pip-index-url-0.1.0/pdm_pip_index_url/__init__.py
--rw-rw-rw-   0        0        0     2721 2023-06-08 10:44:02.000000 pdm-pip-index-url-0.1.0/pdm_pip_index_url/plugin.py
--rw-rw-rw-   0        0        0     1469 2023-06-08 10:44:02.000000 pdm-pip-index-url-0.1.0/pdm_pip_index_url/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-08 11:02:51.391143 pdm-pip-index-url-0.1.0/pdm_pip_index_url.egg-info/
--rw-rw-rw-   0        0        0      946 2023-06-08 11:02:51.000000 pdm-pip-index-url-0.1.0/pdm_pip_index_url.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      358 2023-06-08 11:02:51.000000 pdm-pip-index-url-0.1.0/pdm_pip_index_url.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 11:02:51.000000 pdm-pip-index-url-0.1.0/pdm_pip_index_url.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-06-08 11:02:51.000000 pdm-pip-index-url-0.1.0/pdm_pip_index_url.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       18 2023-06-08 11:02:51.000000 pdm-pip-index-url-0.1.0/pdm_pip_index_url.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      902 2023-06-08 11:02:03.000000 pdm-pip-index-url-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-08 11:02:51.395123 pdm-pip-index-url-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-08 11:02:51.391143 pdm-pip-index-url-0.1.0/tests/
--rw-rw-rw-   0        0        0     4903 2023-06-08 10:44:02.000000 pdm-pip-index-url-0.1.0/tests/test_plugin.py
--rw-rw-rw-   0        0        0     1638 2023-06-08 10:44:02.000000 pdm-pip-index-url-0.1.0/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-08 11:14:08.259436 pdm-pip-index-url-0.1.1/
+-rw-rw-rw-   0        0        0      950 2023-06-08 11:14:08.259436 pdm-pip-index-url-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      603 2023-06-08 10:46:57.000000 pdm-pip-index-url-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 11:14:08.243246 pdm-pip-index-url-0.1.1/pdm_pip_index_url/
+-rw-rw-rw-   0        0        0      201 2023-06-08 10:44:02.000000 pdm-pip-index-url-0.1.1/pdm_pip_index_url/__init__.py
+-rw-rw-rw-   0        0        0     2721 2023-06-08 10:44:02.000000 pdm-pip-index-url-0.1.1/pdm_pip_index_url/plugin.py
+-rw-rw-rw-   0        0        0     1469 2023-06-08 10:44:02.000000 pdm-pip-index-url-0.1.1/pdm_pip_index_url/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-08 11:14:08.255437 pdm-pip-index-url-0.1.1/pdm_pip_index_url.egg-info/
+-rw-rw-rw-   0        0        0      950 2023-06-08 11:14:08.000000 pdm-pip-index-url-0.1.1/pdm_pip_index_url.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      358 2023-06-08 11:14:08.000000 pdm-pip-index-url-0.1.1/pdm_pip_index_url.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 11:14:08.000000 pdm-pip-index-url-0.1.1/pdm_pip_index_url.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-06-08 11:14:08.000000 pdm-pip-index-url-0.1.1/pdm_pip_index_url.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       18 2023-06-08 11:14:08.000000 pdm-pip-index-url-0.1.1/pdm_pip_index_url.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      906 2023-06-08 11:13:34.000000 pdm-pip-index-url-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-08 11:14:08.259436 pdm-pip-index-url-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-08 11:14:08.259436 pdm-pip-index-url-0.1.1/tests/
+-rw-rw-rw-   0        0        0     4903 2023-06-08 10:44:02.000000 pdm-pip-index-url-0.1.1/tests/test_plugin.py
+-rw-rw-rw-   0        0        0     1638 2023-06-08 10:44:02.000000 pdm-pip-index-url-0.1.1/tests/test_utils.py
```

### Comparing `pdm-pip-index-url-0.1.0/PKG-INFO` & `pdm-pip-index-url-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pdm-pip-index-url
-Version: 0.1.0
-Summary: Automatic coverter of PIP_*INDEX_URL to PDM_PYPI_* envs.
+Version: 0.1.1
+Summary: An automatic converter of PIP_*INDEX_URL to PDM_PYPI_* envs.
 Author-email: Kamil Janiec <kamil.p.janiec@gmail.com>
 License: MIT
 Project-URL: repository, https://github.com/theredfoxlee/pdm-pip-index-url
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # pdm-pip-index-url
```

### Comparing `pdm-pip-index-url-0.1.0/README.md` & `pdm-pip-index-url-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pdm-pip-index-url-0.1.0/pdm_pip_index_url/plugin.py` & `pdm-pip-index-url-0.1.1/pdm_pip_index_url/plugin.py`

 * *Files identical despite different names*

### Comparing `pdm-pip-index-url-0.1.0/pdm_pip_index_url/utils.py` & `pdm-pip-index-url-0.1.1/pdm_pip_index_url/utils.py`

 * *Files identical despite different names*

### Comparing `pdm-pip-index-url-0.1.0/pdm_pip_index_url.egg-info/PKG-INFO` & `pdm-pip-index-url-0.1.1/pdm_pip_index_url.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pdm-pip-index-url
-Version: 0.1.0
-Summary: Automatic coverter of PIP_*INDEX_URL to PDM_PYPI_* envs.
+Version: 0.1.1
+Summary: An automatic converter of PIP_*INDEX_URL to PDM_PYPI_* envs.
 Author-email: Kamil Janiec <kamil.p.janiec@gmail.com>
 License: MIT
 Project-URL: repository, https://github.com/theredfoxlee/pdm-pip-index-url
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # pdm-pip-index-url
```

### Comparing `pdm-pip-index-url-0.1.0/pyproject.toml` & `pdm-pip-index-url-0.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 [project]
 name = "pdm-pip-index-url"
-version = "0.1.0"
-description = "Automatic coverter of PIP_*INDEX_URL to PDM_PYPI_* envs."
+version = "0.1.1"
+description = "An automatic converter of PIP_*INDEX_URL to PDM_PYPI_* envs."
 authors = [
     {name = "Kamil Janiec", email = "kamil.p.janiec@gmail.com"},
 ]
 dependencies = [
 ]
 requires-python = ">=3.7"
 readme = "README.md"
```

### Comparing `pdm-pip-index-url-0.1.0/tests/test_plugin.py` & `pdm-pip-index-url-0.1.1/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `pdm-pip-index-url-0.1.0/tests/test_utils.py` & `pdm-pip-index-url-0.1.1/tests/test_utils.py`

 * *Files identical despite different names*

