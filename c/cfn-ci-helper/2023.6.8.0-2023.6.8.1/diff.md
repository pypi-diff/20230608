# Comparing `tmp/cfn-ci-helper-2023.6.8.0.tar.gz` & `tmp/cfn-ci-helper-2023.6.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfn-ci-helper-2023.6.8.0.tar", last modified: Thu Jun  8 16:42:36 2023, max compression
+gzip compressed data, was "cfn-ci-helper-2023.6.8.1.tar", last modified: Thu Jun  8 18:34:55 2023, max compression
```

## Comparing `cfn-ci-helper-2023.6.8.0.tar` & `cfn-ci-helper-2023.6.8.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:42:36.493594 cfn-ci-helper-2023.6.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-08 16:42:17.000000 cfn-ci-helper-2023.6.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 16:42:17.000000 cfn-ci-helper-2023.6.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-08 16:42:36.493594 cfn-ci-helper-2023.6.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-08 16:42:17.000000 cfn-ci-helper-2023.6.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:42:36.489594 cfn-ci-helper-2023.6.8.0/cfnStack/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-08 16:42:17.000000 cfn-ci-helper-2023.6.8.0/cfnStack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-08 16:42:17.000000 cfn-ci-helper-2023.6.8.0/cfnStack/default_stack.yaml.jinja
--rw-r--r--   0 runner    (1001) docker     (123)    16654 2023-06-08 16:42:17.000000 cfn-ci-helper-2023.6.8.0/cfnStack/stack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:42:36.493594 cfn-ci-helper-2023.6.8.0/cfn_ci_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-08 16:42:36.000000 cfn-ci-helper-2023.6.8.0/cfn_ci_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-08 16:42:36.000000 cfn-ci-helper-2023.6.8.0/cfn_ci_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 16:42:36.000000 cfn-ci-helper-2023.6.8.0/cfn_ci_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-08 16:42:36.000000 cfn-ci-helper-2023.6.8.0/cfn_ci_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-08 16:42:36.000000 cfn-ci-helper-2023.6.8.0/cfn_ci_helper.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    10497 2023-06-08 16:42:17.000000 cfn-ci-helper-2023.6.8.0/deploy_cf.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-08 16:42:17.000000 cfn-ci-helper-2023.6.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-08 16:42:36.493594 cfn-ci-helper-2023.6.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:34:55.428159 cfn-ci-helper-2023.6.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-08 18:34:36.000000 cfn-ci-helper-2023.6.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 18:34:36.000000 cfn-ci-helper-2023.6.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-08 18:34:55.428159 cfn-ci-helper-2023.6.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-08 18:34:36.000000 cfn-ci-helper-2023.6.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:34:55.428159 cfn-ci-helper-2023.6.8.1/cfnStack/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-08 18:34:36.000000 cfn-ci-helper-2023.6.8.1/cfnStack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-08 18:34:36.000000 cfn-ci-helper-2023.6.8.1/cfnStack/default_stack.yaml.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)    16676 2023-06-08 18:34:36.000000 cfn-ci-helper-2023.6.8.1/cfnStack/stack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:34:55.428159 cfn-ci-helper-2023.6.8.1/cfn_ci_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-08 18:34:55.000000 cfn-ci-helper-2023.6.8.1/cfn_ci_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-08 18:34:55.000000 cfn-ci-helper-2023.6.8.1/cfn_ci_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 18:34:55.000000 cfn-ci-helper-2023.6.8.1/cfn_ci_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-08 18:34:55.000000 cfn-ci-helper-2023.6.8.1/cfn_ci_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-08 18:34:55.000000 cfn-ci-helper-2023.6.8.1/cfn_ci_helper.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10497 2023-06-08 18:34:36.000000 cfn-ci-helper-2023.6.8.1/deploy_cf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-08 18:34:36.000000 cfn-ci-helper-2023.6.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-08 18:34:55.432160 cfn-ci-helper-2023.6.8.1/setup.cfg
```

### Comparing `cfn-ci-helper-2023.6.8.0/LICENSE` & `cfn-ci-helper-2023.6.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cfn-ci-helper-2023.6.8.0/PKG-INFO` & `cfn-ci-helper-2023.6.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfn-ci-helper
-Version: 2023.6.8.0
+Version: 2023.6.8.1
 Summary: A Cloudformation CI Helper System
 Home-page: https://github.com/chalbersma/cfn-ci-helper
 Author: Chris Halbersma
 Author-email: chris@halbersma.us
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `cfn-ci-helper-2023.6.8.0/cfnStack/default_stack.yaml.jinja` & `cfn-ci-helper-2023.6.8.1/cfnStack/default_stack.yaml.jinja`

 * *Files identical despite different names*

### Comparing `cfn-ci-helper-2023.6.8.0/cfnStack/stack.py` & `cfn-ci-helper-2023.6.8.1/cfnStack/stack.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
                                   aws="Unknown", stack_valid="Unknown",
                                   changes="Unknown", action="Nothing", fail=False)
 
         if self.stack_cfg.get("dynamic_name", False) is not False and isinstance(self.stack_cfg.get("dynamic_name", False), str):
 
             dynamic_okay = True
             # Expand Stack Name With Parameterized Data
-            template_objs = {**self.kwargs.get("live_add", {}),
+            template_objs = {**self.kwargs.get("live_add", {}).get("parameters", {}),
                              **{x["ParameterKey"]: x["ParameterValue"] for x in
                                 self.stack_cfg.get("parameters", list())},
                              **{x["Key"]: x["Value"] for x in self.stack_cfg.get("tags", list())}
                              }
 
             template = string.Template(self.stack_cfg["dynamic_name"])
```

### Comparing `cfn-ci-helper-2023.6.8.0/cfn_ci_helper.egg-info/PKG-INFO` & `cfn-ci-helper-2023.6.8.1/cfn_ci_helper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfn-ci-helper
-Version: 2023.6.8.0
+Version: 2023.6.8.1
 Summary: A Cloudformation CI Helper System
 Home-page: https://github.com/chalbersma/cfn-ci-helper
 Author: Chris Halbersma
 Author-email: chris@halbersma.us
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `cfn-ci-helper-2023.6.8.0/deploy_cf.py` & `cfn-ci-helper-2023.6.8.1/deploy_cf.py`

 * *Files identical despite different names*

### Comparing `cfn-ci-helper-2023.6.8.0/setup.cfg` & `cfn-ci-helper-2023.6.8.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cfn-ci-helper
-version = 2023.06.08.0
+version = 2023.06.08.1
 author = Chris Halbersma
 author_email = chris@halbersma.us
 description = A Cloudformation CI Helper System
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/chalbersma/cfn-ci-helper
 classifiers =
```

