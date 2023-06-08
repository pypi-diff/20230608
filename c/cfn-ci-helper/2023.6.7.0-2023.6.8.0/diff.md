# Comparing `tmp/cfn-ci-helper-2023.6.7.0.tar.gz` & `tmp/cfn-ci-helper-2023.6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfn-ci-helper-2023.6.7.0.tar", last modified: Thu Jun  8 06:21:49 2023, max compression
+gzip compressed data, was "cfn-ci-helper-2023.6.8.0.tar", last modified: Thu Jun  8 16:42:36 2023, max compression
```

## Comparing `cfn-ci-helper-2023.6.7.0.tar` & `cfn-ci-helper-2023.6.8.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:21:49.210377 cfn-ci-helper-2023.6.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-08 06:21:27.000000 cfn-ci-helper-2023.6.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 06:21:27.000000 cfn-ci-helper-2023.6.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-08 06:21:49.210377 cfn-ci-helper-2023.6.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-08 06:21:27.000000 cfn-ci-helper-2023.6.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:21:49.210377 cfn-ci-helper-2023.6.7.0/cfnStack/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-08 06:21:27.000000 cfn-ci-helper-2023.6.7.0/cfnStack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-08 06:21:27.000000 cfn-ci-helper-2023.6.7.0/cfnStack/default_stack.yaml.jinja
--rw-r--r--   0 runner    (1001) docker     (123)    16478 2023-06-08 06:21:27.000000 cfn-ci-helper-2023.6.7.0/cfnStack/stack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:21:49.210377 cfn-ci-helper-2023.6.7.0/cfn_ci_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-08 06:21:49.000000 cfn-ci-helper-2023.6.7.0/cfn_ci_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-08 06:21:49.000000 cfn-ci-helper-2023.6.7.0/cfn_ci_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 06:21:49.000000 cfn-ci-helper-2023.6.7.0/cfn_ci_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-08 06:21:49.000000 cfn-ci-helper-2023.6.7.0/cfn_ci_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-08 06:21:49.000000 cfn-ci-helper-2023.6.7.0/cfn_ci_helper.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    10497 2023-06-08 06:21:27.000000 cfn-ci-helper-2023.6.7.0/deploy_cf.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-08 06:21:27.000000 cfn-ci-helper-2023.6.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-08 06:21:49.214377 cfn-ci-helper-2023.6.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:42:36.493594 cfn-ci-helper-2023.6.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-08 16:42:17.000000 cfn-ci-helper-2023.6.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 16:42:17.000000 cfn-ci-helper-2023.6.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-08 16:42:36.493594 cfn-ci-helper-2023.6.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-08 16:42:17.000000 cfn-ci-helper-2023.6.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:42:36.489594 cfn-ci-helper-2023.6.8.0/cfnStack/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-08 16:42:17.000000 cfn-ci-helper-2023.6.8.0/cfnStack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-08 16:42:17.000000 cfn-ci-helper-2023.6.8.0/cfnStack/default_stack.yaml.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)    16654 2023-06-08 16:42:17.000000 cfn-ci-helper-2023.6.8.0/cfnStack/stack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:42:36.493594 cfn-ci-helper-2023.6.8.0/cfn_ci_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-08 16:42:36.000000 cfn-ci-helper-2023.6.8.0/cfn_ci_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-08 16:42:36.000000 cfn-ci-helper-2023.6.8.0/cfn_ci_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 16:42:36.000000 cfn-ci-helper-2023.6.8.0/cfn_ci_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-08 16:42:36.000000 cfn-ci-helper-2023.6.8.0/cfn_ci_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-08 16:42:36.000000 cfn-ci-helper-2023.6.8.0/cfn_ci_helper.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10497 2023-06-08 16:42:17.000000 cfn-ci-helper-2023.6.8.0/deploy_cf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-08 16:42:17.000000 cfn-ci-helper-2023.6.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-08 16:42:36.493594 cfn-ci-helper-2023.6.8.0/setup.cfg
```

### Comparing `cfn-ci-helper-2023.6.7.0/LICENSE` & `cfn-ci-helper-2023.6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cfn-ci-helper-2023.6.7.0/PKG-INFO` & `cfn-ci-helper-2023.6.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfn-ci-helper
-Version: 2023.6.7.0
+Version: 2023.6.8.0
 Summary: A Cloudformation CI Helper System
 Home-page: https://github.com/chalbersma/cfn-ci-helper
 Author: Chris Halbersma
 Author-email: chris@halbersma.us
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `cfn-ci-helper-2023.6.7.0/cfnStack/default_stack.yaml.jinja` & `cfn-ci-helper-2023.6.8.0/cfnStack/default_stack.yaml.jinja`

 * *Files identical despite different names*

### Comparing `cfn-ci-helper-2023.6.7.0/cfnStack/stack.py` & `cfn-ci-helper-2023.6.8.0/cfnStack/stack.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,43 +37,44 @@
         self.go = True
 
         self.return_status = dict(stack=self.stack_name,
                                   profile=self.aws_profile,
                                   aws="Unknown", stack_valid="Unknown",
                                   changes="Unknown", action="Nothing", fail=False)
 
-        if self.stack_cfg.get("dynamic_name", False) is True:
+        if self.stack_cfg.get("dynamic_name", False) is not False and isinstance(self.stack_cfg.get("dynamic_name", False), str):
 
             dynamic_okay = True
             # Expand Stack Name With Parameterized Data
             template_objs = {**self.kwargs.get("live_add", {}),
                              **{x["ParameterKey"]: x["ParameterValue"] for x in
                                 self.stack_cfg.get("parameters", list())},
                              **{x["Key"]: x["Value"] for x in self.stack_cfg.get("tags", list())}
                              }
 
-            template = string.Template(self.stack_name)
+            template = string.Template(self.stack_cfg["dynamic_name"])
 
             try:
                 self.stack_name = template.substitute(mappings=template_objs)
             except Exception as TemplateError:
-                self.logger.error("Error doing Dynamic Name Substitution : {}")
-                self.logger.info("Template : {}".format(stack_config["stack"]))
+                self.logger.error("Error doing Dynamic Name Substitution : {}".format(TemplateError))
+                self.logger.info("Template : {}".format(self.stack_cfg["dynamic_name"]))
                 self.logger.debug("Available Replacements : {}".format(template_objs))
 
                 self.go = False
                 dynamic_okay = False
                 self.return_status["stack_valid"] = "Dynamic Name Failure"
                 self.return_status["fail"] = True
 
             else:
-                self.logger.info("Dynamic Name Went from : {} to {}".format(stack_config["stack"], self.stack_name))
+                self.logger.info("Dynamic Name Went from : {} to {}".format(self.stack_cfg["dynamic_name"], self.stack_name))
                 self.return_status["stack"] = self.stack_name
         else:
             # No Dynamic Name Used
+            self.logger.info("No Dynamic Name Used")
             dynamic_okay = True
 
         region_text = str()
         if self.region != self._region:
             region_text = "[{}]".format(self.region)
         self.lname = "{}/{}{}".format(self.stack_name, self.aws_profile, region_text)
```

### Comparing `cfn-ci-helper-2023.6.7.0/cfn_ci_helper.egg-info/PKG-INFO` & `cfn-ci-helper-2023.6.8.0/cfn_ci_helper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfn-ci-helper
-Version: 2023.6.7.0
+Version: 2023.6.8.0
 Summary: A Cloudformation CI Helper System
 Home-page: https://github.com/chalbersma/cfn-ci-helper
 Author: Chris Halbersma
 Author-email: chris@halbersma.us
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `cfn-ci-helper-2023.6.7.0/deploy_cf.py` & `cfn-ci-helper-2023.6.8.0/deploy_cf.py`

 * *Files identical despite different names*

### Comparing `cfn-ci-helper-2023.6.7.0/setup.cfg` & `cfn-ci-helper-2023.6.8.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cfn-ci-helper
-version = 2023.06.07.0
+version = 2023.06.08.0
 author = Chris Halbersma
 author_email = chris@halbersma.us
 description = A Cloudformation CI Helper System
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/chalbersma/cfn-ci-helper
 classifiers =
```

