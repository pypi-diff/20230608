# Comparing `tmp/ssm-ps-template-2.2.0.tar.gz` & `tmp/ssm-ps-template-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssm-ps-template-2.2.0.tar", last modified: Tue Jun  6 18:35:06 2023, max compression
+gzip compressed data, was "ssm-ps-template-2.3.0.tar", last modified: Thu Jun  8 21:23:46 2023, max compression
```

## Comparing `ssm-ps-template-2.2.0.tar` & `ssm-ps-template-2.3.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 18:35:06.668367 ssm-ps-template-2.2.0/
--rw-r--r--   0 root         (0) root         (0)     1495 2023-06-06 18:34:57.000000 ssm-ps-template-2.2.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    12040 2023-06-06 18:35:06.668367 ssm-ps-template-2.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9404 2023-06-06 18:34:57.000000 ssm-ps-template-2.2.0/README.md
--rw-r--r--   0 root         (0) root         (0)     1879 2023-06-06 18:34:57.000000 ssm-ps-template-2.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 18:35:06.668367 ssm-ps-template-2.2.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 18:35:06.668367 ssm-ps-template-2.2.0/ssm_ps_template/
--rw-r--r--   0 root         (0) root         (0)      148 2023-06-06 18:34:57.000000 ssm-ps-template-2.2.0/ssm_ps_template/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3254 2023-06-06 18:34:57.000000 ssm-ps-template-2.2.0/ssm_ps_template/__main__.py
--rw-r--r--   0 root         (0) root         (0)     2364 2023-06-06 18:34:57.000000 ssm-ps-template-2.2.0/ssm_ps_template/config.py
--rw-r--r--   0 root         (0) root         (0)     1825 2023-06-06 18:34:57.000000 ssm-ps-template-2.2.0/ssm_ps_template/discovery.py
--rw-r--r--   0 root         (0) root         (0)     2686 2023-06-06 18:34:57.000000 ssm-ps-template-2.2.0/ssm_ps_template/render.py
--rw-r--r--   0 root         (0) root         (0)     3388 2023-06-06 18:34:57.000000 ssm-ps-template-2.2.0/ssm_ps_template/ssm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 18:35:06.668367 ssm-ps-template-2.2.0/ssm_ps_template.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12040 2023-06-06 18:35:06.000000 ssm-ps-template-2.2.0/ssm_ps_template.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      535 2023-06-06 18:35:06.000000 ssm-ps-template-2.2.0/ssm_ps_template.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 18:35:06.000000 ssm-ps-template-2.2.0/ssm_ps_template.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2023-06-06 18:35:06.000000 ssm-ps-template-2.2.0/ssm_ps_template.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      246 2023-06-06 18:35:06.000000 ssm-ps-template-2.2.0/ssm_ps_template.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-06 18:35:06.000000 ssm-ps-template-2.2.0/ssm_ps_template.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 18:35:06.668367 ssm-ps-template-2.2.0/tests/
--rw-r--r--   0 root         (0) root         (0)     2833 2023-06-06 18:34:57.000000 ssm-ps-template-2.2.0/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)      784 2023-06-06 18:34:57.000000 ssm-ps-template-2.2.0/tests/test_discovery.py
--rw-r--r--   0 root         (0) root         (0)     1332 2023-06-06 18:34:57.000000 ssm-ps-template-2.2.0/tests/test_main.py
--rw-r--r--   0 root         (0) root         (0)     2191 2023-06-06 18:34:57.000000 ssm-ps-template-2.2.0/tests/test_render.py
--rw-r--r--   0 root         (0) root         (0)     3119 2023-06-06 18:34:57.000000 ssm-ps-template-2.2.0/tests/test_ssm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 21:23:46.932765 ssm-ps-template-2.3.0/
+-rw-r--r--   0 root         (0) root         (0)     1495 2023-06-08 21:23:35.000000 ssm-ps-template-2.3.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    12318 2023-06-08 21:23:46.932765 ssm-ps-template-2.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9682 2023-06-08 21:23:35.000000 ssm-ps-template-2.3.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1879 2023-06-08 21:23:35.000000 ssm-ps-template-2.3.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 21:23:46.932765 ssm-ps-template-2.3.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 21:23:46.928764 ssm-ps-template-2.3.0/ssm_ps_template/
+-rw-r--r--   0 root         (0) root         (0)      148 2023-06-08 21:23:35.000000 ssm-ps-template-2.3.0/ssm_ps_template/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3254 2023-06-08 21:23:35.000000 ssm-ps-template-2.3.0/ssm_ps_template/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     2364 2023-06-08 21:23:35.000000 ssm-ps-template-2.3.0/ssm_ps_template/config.py
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-06-08 21:23:35.000000 ssm-ps-template-2.3.0/ssm_ps_template/discovery.py
+-rw-r--r--   0 root         (0) root         (0)     2834 2023-06-08 21:23:35.000000 ssm-ps-template-2.3.0/ssm_ps_template/render.py
+-rw-r--r--   0 root         (0) root         (0)     3388 2023-06-08 21:23:35.000000 ssm-ps-template-2.3.0/ssm_ps_template/ssm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 21:23:46.932765 ssm-ps-template-2.3.0/ssm_ps_template.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12318 2023-06-08 21:23:46.000000 ssm-ps-template-2.3.0/ssm_ps_template.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      535 2023-06-08 21:23:46.000000 ssm-ps-template-2.3.0/ssm_ps_template.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 21:23:46.000000 ssm-ps-template-2.3.0/ssm_ps_template.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-06-08 21:23:46.000000 ssm-ps-template-2.3.0/ssm_ps_template.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      246 2023-06-08 21:23:46.000000 ssm-ps-template-2.3.0/ssm_ps_template.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-08 21:23:46.000000 ssm-ps-template-2.3.0/ssm_ps_template.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 21:23:46.932765 ssm-ps-template-2.3.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     2833 2023-06-08 21:23:35.000000 ssm-ps-template-2.3.0/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)      784 2023-06-08 21:23:35.000000 ssm-ps-template-2.3.0/tests/test_discovery.py
+-rw-r--r--   0 root         (0) root         (0)     1332 2023-06-08 21:23:35.000000 ssm-ps-template-2.3.0/tests/test_main.py
+-rw-r--r--   0 root         (0) root         (0)     2191 2023-06-08 21:23:35.000000 ssm-ps-template-2.3.0/tests/test_render.py
+-rw-r--r--   0 root         (0) root         (0)     3119 2023-06-08 21:23:35.000000 ssm-ps-template-2.3.0/tests/test_ssm.py
```

### Comparing `ssm-ps-template-2.2.0/LICENSE.txt` & `ssm-ps-template-2.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.2.0/PKG-INFO` & `ssm-ps-template-2.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssm-ps-template
-Version: 2.2.0
+Version: 2.3.0
 Summary: CLI for rendering configuration templates with SSM Parameter Store as a data source
 Author-email: "Gavin M. Roy" <gavinmroy@gmail.com>
 License: Copyright (c) 2023 Gavin M. Roy
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
@@ -167,14 +167,16 @@
 | `unquote`                | The [`urllib.parse.unquote`](https://docs.python.org/3/library/urllib.parse.html#urllib.parse.unquote) function from the Python standard library.   |
 
 The following filters are added:
 
 | Filter                  | Description                                                                                                  |
 |-------------------------|--------------------------------------------------------------------------------------------------------------|
 | `dashes_to_underscores` | Recursively replaces dashes with underscores in keys in data structures returned by `get_parameters_by_path` |
+| `fromjson`              | Convert a JSON blob to a data structure                                                                      |
+| `fromyaml`              | Convert a YAML blob to a data structure                                                                      |
 | `path_to_dict`          | Converts a dict with forward-slash delimited keys (`/`) to a nested dict using the `/` as the key delimiter  |
 | `toyaml`                | Converts a dictionary value to YAML                                                                          |
 
 The following variables are exposed:
 
 | Variable  | Definition                                                                                                              |
 |-----------|-------------------------------------------------------------------------------------------------------------------------|
```

### Comparing `ssm-ps-template-2.2.0/README.md` & `ssm-ps-template-2.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -118,14 +118,16 @@
 | `unquote`                | The [`urllib.parse.unquote`](https://docs.python.org/3/library/urllib.parse.html#urllib.parse.unquote) function from the Python standard library.   |
 
 The following filters are added:
 
 | Filter                  | Description                                                                                                  |
 |-------------------------|--------------------------------------------------------------------------------------------------------------|
 | `dashes_to_underscores` | Recursively replaces dashes with underscores in keys in data structures returned by `get_parameters_by_path` |
+| `fromjson`              | Convert a JSON blob to a data structure                                                                      |
+| `fromyaml`              | Convert a YAML blob to a data structure                                                                      |
 | `path_to_dict`          | Converts a dict with forward-slash delimited keys (`/`) to a nested dict using the `/` as the key delimiter  |
 | `toyaml`                | Converts a dictionary value to YAML                                                                          |
 
 The following variables are exposed:
 
 | Variable  | Definition                                                                                                              |
 |-----------|-------------------------------------------------------------------------------------------------------------------------|
```

### Comparing `ssm-ps-template-2.2.0/pyproject.toml` & `ssm-ps-template-2.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ssm-ps-template"
-version = "2.2.0"
+version = "2.3.0"
 description = "CLI for rendering configuration templates with SSM Parameter Store as a data source"
 authors = [
     {name = "Gavin M. Roy", email="gavinmroy@gmail.com"}
 ]
 classifiers = [
     "Topic :: Software Development",
     "License :: OSI Approved :: BSD License",
```

### Comparing `ssm-ps-template-2.2.0/ssm_ps_template/__main__.py` & `ssm-ps-template-2.3.0/ssm_ps_template/__main__.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.2.0/ssm_ps_template/config.py` & `ssm-ps-template-2.3.0/ssm_ps_template/config.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.2.0/ssm_ps_template/discovery.py` & `ssm-ps-template-2.3.0/ssm_ps_template/discovery.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.2.0/ssm_ps_template/render.py` & `ssm-ps-template-2.3.0/ssm_ps_template/render.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import logging
 import os
 import pathlib
 import typing
 from urllib import parse
 
 import flatdict
@@ -50,14 +51,16 @@
 
     def render(self, values: ssm.Values) -> str:
         """Render the template to the internal buffer"""
         self._values = values
         environment = sandbox.ImmutableSandboxedEnvironment()
         environment.filters['dashes_to_underscores'] = \
             replace_dashes_with_underscores
+        environment.filters['fromjson'] = lambda v: json.loads(v)
+        environment.filters['fromyaml'] = lambda v: yaml.safe_load(v)
         environment.filters['path_to_dict'] = path_to_dict
         environment.filters['toyaml'] = lambda v: yaml.safe_dump(v)
         environment.globals['get_parameter'] = self._get_parameter
         environment.globals['get_parameters_by_path'] = \
             self._get_parameters_by_path
         environment.globals['parse_qs'] = parse.parse_qs
         environment.globals['unquote'] = parse.unquote
```

### Comparing `ssm-ps-template-2.2.0/ssm_ps_template/ssm.py` & `ssm-ps-template-2.3.0/ssm_ps_template/ssm.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.2.0/ssm_ps_template.egg-info/PKG-INFO` & `ssm-ps-template-2.3.0/ssm_ps_template.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssm-ps-template
-Version: 2.2.0
+Version: 2.3.0
 Summary: CLI for rendering configuration templates with SSM Parameter Store as a data source
 Author-email: "Gavin M. Roy" <gavinmroy@gmail.com>
 License: Copyright (c) 2023 Gavin M. Roy
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
@@ -167,14 +167,16 @@
 | `unquote`                | The [`urllib.parse.unquote`](https://docs.python.org/3/library/urllib.parse.html#urllib.parse.unquote) function from the Python standard library.   |
 
 The following filters are added:
 
 | Filter                  | Description                                                                                                  |
 |-------------------------|--------------------------------------------------------------------------------------------------------------|
 | `dashes_to_underscores` | Recursively replaces dashes with underscores in keys in data structures returned by `get_parameters_by_path` |
+| `fromjson`              | Convert a JSON blob to a data structure                                                                      |
+| `fromyaml`              | Convert a YAML blob to a data structure                                                                      |
 | `path_to_dict`          | Converts a dict with forward-slash delimited keys (`/`) to a nested dict using the `/` as the key delimiter  |
 | `toyaml`                | Converts a dictionary value to YAML                                                                          |
 
 The following variables are exposed:
 
 | Variable  | Definition                                                                                                              |
 |-----------|-------------------------------------------------------------------------------------------------------------------------|
```

### Comparing `ssm-ps-template-2.2.0/ssm_ps_template.egg-info/SOURCES.txt` & `ssm-ps-template-2.3.0/ssm_ps_template.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.2.0/tests/test_config.py` & `ssm-ps-template-2.3.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.2.0/tests/test_discovery.py` & `ssm-ps-template-2.3.0/tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.2.0/tests/test_main.py` & `ssm-ps-template-2.3.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.2.0/tests/test_render.py` & `ssm-ps-template-2.3.0/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.2.0/tests/test_ssm.py` & `ssm-ps-template-2.3.0/tests/test_ssm.py`

 * *Files identical despite different names*

