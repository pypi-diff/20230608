# Comparing `tmp/cfn-ci-helper-2023.6.8.2.tar.gz` & `tmp/cfn-ci-helper-2023.6.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfn-ci-helper-2023.6.8.2.tar", last modified: Thu Jun  8 18:45:31 2023, max compression
+gzip compressed data, was "cfn-ci-helper-2023.6.8.3.tar", last modified: Thu Jun  8 18:54:39 2023, max compression
```

## Comparing `cfn-ci-helper-2023.6.8.2.tar` & `cfn-ci-helper-2023.6.8.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:45:31.517281 cfn-ci-helper-2023.6.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-08 18:45:10.000000 cfn-ci-helper-2023.6.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 18:45:10.000000 cfn-ci-helper-2023.6.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-08 18:45:31.517281 cfn-ci-helper-2023.6.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-08 18:45:10.000000 cfn-ci-helper-2023.6.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:45:31.517281 cfn-ci-helper-2023.6.8.2/cfnStack/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-08 18:45:10.000000 cfn-ci-helper-2023.6.8.2/cfnStack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-08 18:45:10.000000 cfn-ci-helper-2023.6.8.2/cfnStack/default_stack.yaml.jinja
--rw-r--r--   0 runner    (1001) docker     (123)    16771 2023-06-08 18:45:10.000000 cfn-ci-helper-2023.6.8.2/cfnStack/stack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:45:31.517281 cfn-ci-helper-2023.6.8.2/cfn_ci_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-08 18:45:31.000000 cfn-ci-helper-2023.6.8.2/cfn_ci_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-08 18:45:31.000000 cfn-ci-helper-2023.6.8.2/cfn_ci_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 18:45:31.000000 cfn-ci-helper-2023.6.8.2/cfn_ci_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-08 18:45:31.000000 cfn-ci-helper-2023.6.8.2/cfn_ci_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-08 18:45:31.000000 cfn-ci-helper-2023.6.8.2/cfn_ci_helper.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    10497 2023-06-08 18:45:10.000000 cfn-ci-helper-2023.6.8.2/deploy_cf.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-08 18:45:10.000000 cfn-ci-helper-2023.6.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-08 18:45:31.517281 cfn-ci-helper-2023.6.8.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:54:38.999171 cfn-ci-helper-2023.6.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-08 18:54:22.000000 cfn-ci-helper-2023.6.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 18:54:22.000000 cfn-ci-helper-2023.6.8.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-08 18:54:38.999171 cfn-ci-helper-2023.6.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-08 18:54:22.000000 cfn-ci-helper-2023.6.8.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:54:38.999171 cfn-ci-helper-2023.6.8.3/cfnStack/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-08 18:54:22.000000 cfn-ci-helper-2023.6.8.3/cfnStack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-08 18:54:22.000000 cfn-ci-helper-2023.6.8.3/cfnStack/default_stack.yaml.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)    16771 2023-06-08 18:54:22.000000 cfn-ci-helper-2023.6.8.3/cfnStack/stack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:54:38.999171 cfn-ci-helper-2023.6.8.3/cfn_ci_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-08 18:54:38.000000 cfn-ci-helper-2023.6.8.3/cfn_ci_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-08 18:54:38.000000 cfn-ci-helper-2023.6.8.3/cfn_ci_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 18:54:38.000000 cfn-ci-helper-2023.6.8.3/cfn_ci_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-08 18:54:38.000000 cfn-ci-helper-2023.6.8.3/cfn_ci_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-08 18:54:38.000000 cfn-ci-helper-2023.6.8.3/cfn_ci_helper.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-06-08 18:54:22.000000 cfn-ci-helper-2023.6.8.3/deploy_cf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-08 18:54:22.000000 cfn-ci-helper-2023.6.8.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-08 18:54:38.999171 cfn-ci-helper-2023.6.8.3/setup.cfg
```

### Comparing `cfn-ci-helper-2023.6.8.2/LICENSE` & `cfn-ci-helper-2023.6.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cfn-ci-helper-2023.6.8.2/PKG-INFO` & `cfn-ci-helper-2023.6.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfn-ci-helper
-Version: 2023.6.8.2
+Version: 2023.6.8.3
 Summary: A Cloudformation CI Helper System
 Home-page: https://github.com/chalbersma/cfn-ci-helper
 Author: Chris Halbersma
 Author-email: chris@halbersma.us
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `cfn-ci-helper-2023.6.8.2/cfnStack/default_stack.yaml.jinja` & `cfn-ci-helper-2023.6.8.3/cfnStack/default_stack.yaml.jinja`

 * *Files identical despite different names*

### Comparing `cfn-ci-helper-2023.6.8.2/cfnStack/stack.py` & `cfn-ci-helper-2023.6.8.3/cfnStack/stack.py`

 * *Files identical despite different names*

### Comparing `cfn-ci-helper-2023.6.8.2/cfn_ci_helper.egg-info/PKG-INFO` & `cfn-ci-helper-2023.6.8.3/cfn_ci_helper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfn-ci-helper
-Version: 2023.6.8.2
+Version: 2023.6.8.3
 Summary: A Cloudformation CI Helper System
 Home-page: https://github.com/chalbersma/cfn-ci-helper
 Author: Chris Halbersma
 Author-email: chris@halbersma.us
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `cfn-ci-helper-2023.6.8.2/deploy_cf.py` & `cfn-ci-helper-2023.6.8.3/deploy_cf.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,14 +146,16 @@
                     category_configs = yaml.safe_load(config_rendered)
 
                     logger.debug("configs: {}".format(category_configs))
 
     # Parse Live Add Options
     live_add = dict(parameters={})
 
+    logger.debug(args.parameters)
+
     for param in args.parameters:
 
         param_key, param_val = param.split(":", 1)
         logger.debug("Adding Parameter {}".format(param_key))
         live_add["parameters"][param_key] = param_val
```

### Comparing `cfn-ci-helper-2023.6.8.2/setup.cfg` & `cfn-ci-helper-2023.6.8.3/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cfn-ci-helper
-version = 2023.06.08.2
+version = 2023.6.8.3
 author = Chris Halbersma
 author_email = chris@halbersma.us
 description = A Cloudformation CI Helper System
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/chalbersma/cfn-ci-helper
 classifiers =
```

