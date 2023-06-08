# Comparing `tmp/cfn-ci-helper-2023.5.18.0.tar.gz` & `tmp/cfn-ci-helper-2023.6.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfn-ci-helper-2023.5.18.0.tar", last modified: Thu May 25 21:42:14 2023, max compression
+gzip compressed data, was "cfn-ci-helper-2023.6.7.0.tar", last modified: Thu Jun  8 06:21:49 2023, max compression
```

## Comparing `cfn-ci-helper-2023.5.18.0.tar` & `cfn-ci-helper-2023.6.7.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:42:14.321302 cfn-ci-helper-2023.5.18.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-25 21:41:57.000000 cfn-ci-helper-2023.5.18.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-25 21:41:57.000000 cfn-ci-helper-2023.5.18.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-25 21:42:14.321302 cfn-ci-helper-2023.5.18.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-25 21:41:57.000000 cfn-ci-helper-2023.5.18.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:42:14.317302 cfn-ci-helper-2023.5.18.0/cfnStack/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-25 21:41:57.000000 cfn-ci-helper-2023.5.18.0/cfnStack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-25 21:41:57.000000 cfn-ci-helper-2023.5.18.0/cfnStack/default_stack.yaml.jinja
--rw-r--r--   0 runner    (1001) docker     (123)    14738 2023-05-25 21:41:57.000000 cfn-ci-helper-2023.5.18.0/cfnStack/stack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:42:14.321302 cfn-ci-helper-2023.5.18.0/cfn_ci_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-25 21:42:14.000000 cfn-ci-helper-2023.5.18.0/cfn_ci_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-25 21:42:14.000000 cfn-ci-helper-2023.5.18.0/cfn_ci_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 21:42:14.000000 cfn-ci-helper-2023.5.18.0/cfn_ci_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-25 21:42:14.000000 cfn-ci-helper-2023.5.18.0/cfn_ci_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 21:42:14.000000 cfn-ci-helper-2023.5.18.0/cfn_ci_helper.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    10497 2023-05-25 21:41:57.000000 cfn-ci-helper-2023.5.18.0/deploy_cf.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-25 21:41:57.000000 cfn-ci-helper-2023.5.18.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-25 21:42:14.321302 cfn-ci-helper-2023.5.18.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:21:49.210377 cfn-ci-helper-2023.6.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-08 06:21:27.000000 cfn-ci-helper-2023.6.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 06:21:27.000000 cfn-ci-helper-2023.6.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-08 06:21:49.210377 cfn-ci-helper-2023.6.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-08 06:21:27.000000 cfn-ci-helper-2023.6.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:21:49.210377 cfn-ci-helper-2023.6.7.0/cfnStack/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-08 06:21:27.000000 cfn-ci-helper-2023.6.7.0/cfnStack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-08 06:21:27.000000 cfn-ci-helper-2023.6.7.0/cfnStack/default_stack.yaml.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)    16478 2023-06-08 06:21:27.000000 cfn-ci-helper-2023.6.7.0/cfnStack/stack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:21:49.210377 cfn-ci-helper-2023.6.7.0/cfn_ci_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-08 06:21:49.000000 cfn-ci-helper-2023.6.7.0/cfn_ci_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-08 06:21:49.000000 cfn-ci-helper-2023.6.7.0/cfn_ci_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 06:21:49.000000 cfn-ci-helper-2023.6.7.0/cfn_ci_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-08 06:21:49.000000 cfn-ci-helper-2023.6.7.0/cfn_ci_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-08 06:21:49.000000 cfn-ci-helper-2023.6.7.0/cfn_ci_helper.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10497 2023-06-08 06:21:27.000000 cfn-ci-helper-2023.6.7.0/deploy_cf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-08 06:21:27.000000 cfn-ci-helper-2023.6.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-08 06:21:49.214377 cfn-ci-helper-2023.6.7.0/setup.cfg
```

### Comparing `cfn-ci-helper-2023.5.18.0/LICENSE` & `cfn-ci-helper-2023.6.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cfn-ci-helper-2023.5.18.0/PKG-INFO` & `cfn-ci-helper-2023.6.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfn-ci-helper
-Version: 2023.5.18.0
+Version: 2023.6.7.0
 Summary: A Cloudformation CI Helper System
 Home-page: https://github.com/chalbersma/cfn-ci-helper
 Author: Chris Halbersma
 Author-email: chris@halbersma.us
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `cfn-ci-helper-2023.5.18.0/cfnStack/default_stack.yaml.jinja` & `cfn-ci-helper-2023.6.7.0/cfnStack/default_stack.yaml.jinja`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 ---
 default:
   file: {{ filename }}
   description: {{ description }}
+  dynamic_name: {{ dynamic_name|default("false", true) }}
   {% if capabilities|length > 0 %}
   capabilities:
     {% for capability in capabilities %}
     - {{ capability }}
     {% endfor %}
   {% endif %}
   {% if tags|length > 0 -%}
```

### Comparing `cfn-ci-helper-2023.5.18.0/cfnStack/stack.py` & `cfn-ci-helper-2023.6.7.0/cfnStack/stack.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 #!/usr/bin/env python3
 
 import logging
 import time
 import datetime
+import string
 
 import boto3
 from botocore.exceptions import ClientError
 
-class ProcessStack:
 
+class ProcessStack:
     _timeout = 180
     _region = "us-west-2"
     _valid_capabilities = ["CAPABILITY_IAM", "CAPABILITY_NAMED_IAM", "CAPABILITY_AUTO_EXPAND"]
 
     def __init__(self, stack_config, confirm=False,
                  timeout=_timeout, region=_region,
                  **kwargs):
@@ -29,41 +30,72 @@
         if self.aws_profile == "default":
             # To use the default profile set to None
             self.aws_profile = None
 
         self.confirm = confirm
         self.timeout = timeout
 
-        region_text = str()
-        if self.region != self._region:
-            region_text = "[{}]".format(self.region)
-        self.lname = "{}/{}{}".format(self.stack_name, self.aws_profile, region_text)
-
-        self.extend_live_add()
+        self.go = True
 
         self.return_status = dict(stack=self.stack_name,
                                   profile=self.aws_profile,
                                   aws="Unknown", stack_valid="Unknown",
                                   changes="Unknown", action="Nothing", fail=False)
 
-        self.go = True
+        if self.stack_cfg.get("dynamic_name", False) is True:
+
+            dynamic_okay = True
+            # Expand Stack Name With Parameterized Data
+            template_objs = {**self.kwargs.get("live_add", {}),
+                             **{x["ParameterKey"]: x["ParameterValue"] for x in
+                                self.stack_cfg.get("parameters", list())},
+                             **{x["Key"]: x["Value"] for x in self.stack_cfg.get("tags", list())}
+                             }
+
+            template = string.Template(self.stack_name)
+
+            try:
+                self.stack_name = template.substitute(mappings=template_objs)
+            except Exception as TemplateError:
+                self.logger.error("Error doing Dynamic Name Substitution : {}")
+                self.logger.info("Template : {}".format(stack_config["stack"]))
+                self.logger.debug("Available Replacements : {}".format(template_objs))
+
+                self.go = False
+                dynamic_okay = False
+                self.return_status["stack_valid"] = "Dynamic Name Failure"
+                self.return_status["fail"] = True
+
+            else:
+                self.logger.info("Dynamic Name Went from : {} to {}".format(stack_config["stack"], self.stack_name))
+                self.return_status["stack"] = self.stack_name
+        else:
+            # No Dynamic Name Used
+            dynamic_okay = True
+
+        region_text = str()
+        if self.region != self._region:
+            region_text = "[{}]".format(self.region)
+        self.lname = "{}/{}{}".format(self.stack_name, self.aws_profile, region_text)
+
+        self.extend_live_add()
 
         if self.go:
             self.cf_client = self.get_client()
 
         if self.go:
             self.clean_change_sets()
 
         if self.go:
             self.validate_stack()
 
         if self.go:
             self.process_changeset()
 
-        #self.clean_change_sets()
+        # self.clean_change_sets()
 
     def extend_live_add(self):
 
         live_add = self.kwargs.get("live_add", {})
 
         for key, value in live_add.items():
             if key == "parameters":
@@ -89,26 +121,30 @@
 
             changesets = self.cf_client.list_change_sets(StackName=self.stack_name)
 
             outstanding_changesets = len(changesets["Summaries"])
 
             if outstanding_changesets > 0:
                 for this_changeset in changesets["Summaries"]:
-                    self.logger.info("{} Cleaning Changeset named : {}".format(self.lname, this_changeset["ChangeSetName"]))
+                    self.logger.info(
+                        "{} Cleaning Changeset named : {}".format(self.lname, this_changeset["ChangeSetName"]))
 
                     try:
                         self.cf_client.delete_change_set(ChangeSetName=this_changeset["ChangeSetId"])
                     except Exception as delete_error:
-                        self.logger.warning("{} Unable to Delete old Chnageset {}. Hanging Changeset".format(self.lname, this_changeset["ChangeSetName"]))
+                        self.logger.warning("{} Unable to Delete old Chnageset {}. Hanging Changeset".format(self.lname,
+                                                                                                             this_changeset[
+                                                                                                                 "ChangeSetName"]))
                         self.logger.debug("Error: {}".format(delete_error))
                         self.logger.warning("{} Continuing with Hanging Changeset, Clean Manually".format(self.lname))
                         self.go = False
                         self.return_status["fail"] = True
                     else:
-                        self.logger.info("{} Successfully Deleted Changeset {}".format(self.lname, this_changeset["ChangeSetName"]))
+                        self.logger.info(
+                            "{} Successfully Deleted Changeset {}".format(self.lname, this_changeset["ChangeSetName"]))
             else:
                 self.logger.info("{} No Oustanding Changests to Clean".format(self.lname))
         else:
             self.logger.info("{} New Stack, no outstanding changesets to remove.".format(self.lname))
 
     def return_table_row(self):
 
@@ -139,15 +175,16 @@
 
         # Validate OKAY Region
 
         try:
             aws_session = boto3.session.Session(profile_name=self.aws_profile, region_name=self.region)
             cf_client = aws_session.client("cloudformation")
         except Exception as error:
-            self.logger.error("Unable to Provision a Cloudformation Client in AWS Profile : {}".format(self.aws_profile))
+            self.logger.error(
+                "Unable to Provision a Cloudformation Client in AWS Profile : {}".format(self.aws_profile))
             self.logger.debug("Error on Session: {}".format(error))
             self.return_status["aws"] = "Error"
             self.go = False
             self.return_status["fail"] = True
             cf_client = None
         else:
             self.return_status["aws"] = self.aws_profile
@@ -179,27 +216,24 @@
         if len(invalid) > 0:
             self.logger.error("Found {} invalid capabilities.".format(len(invalid)))
             self.logger.debug("Invalid Capabilities : {}".format(", ".join(invalid)))
             cap_okay = False
 
         return cap_okay
 
-
-
     def validate_stack(self):
 
         """
         Validate Stack Being Okay
         :return:
         """
 
         # Validate Stack
         self.logger.info("{} : Validating Stack Template".format(self.lname))
 
-
         try:
             self.cf_client.validate_template(TemplateBody=self.stack_config_json)
         except Exception as ValidationError:
             self.logger.error("Unable to Validate Template for {}.".format(self.lname))
             self.logger.debug("Error on Validation: {}".format(ValidationError))
             self.return_status["stack_valid"] = "Invalid"
             self.return_status["fail"] = True
@@ -275,15 +309,14 @@
             else:
                 raise TypeError("Unknown Status {}".format(current_status))
 
             time.sleep(2)
 
         return complete
 
-
     def process_changeset(self):
 
         """
         Process Changeset
 
         :return:
         """
@@ -297,15 +330,16 @@
                         "Capabilities": self.stack_cfg.get("capabilities", list()),
                         "Tags": self.stack_cfg.get("tags", list()),
                         "Description": self.stack_cfg.get("description", "No Description Given")
                         }
 
         self.logger.debug("{} general_args: {}".format(self.lname, general_args))
 
-        changeset_name = datetime.datetime.today().strftime("{}-{}-%Y-%m-%d-%s".format(self.stack_name, self.aws_profile))
+        changeset_name = datetime.datetime.today().strftime(
+            "{}-{}-%Y-%m-%d-%s".format(self.stack_name, self.aws_profile))
 
         self.logger.info("{} Creating Changeset {}".format(self.lname, changeset_name))
 
         if self.delete is False:
             # Make Changeset to Calculate Changes
 
             changeset_ident = self.cf_client.create_change_set(ChangeSetName=changeset_name,
@@ -334,30 +368,29 @@
             # Delete Reequested
             pending_change = 1
             self.return_status["changes"] = "1 Delete"
             if cstype == "DELETED":
                 pending_change = 0
                 self.return_status["changes"] = "None (Del)"
 
-
         if self.confirm is True and pending_change > 0 and self.delete is False:
             # Do Change
 
             cs_complete = self.wait_for_complete(changeset_ident["Id"])
             if cs_complete != "yes":
                 self.logger.error("Unable to create a changeset {}".format(cs_complete))
                 self.return_status["changes"] = "Error Creating ChangeSet"
                 self.return_status["fail"] = True
                 self.go = False
                 return
 
             self.logger.info("{} : Executing {} Changes".format(self.lname, pending_change))
             self.cf_client.execute_change_set(ChangeSetName=changeset_ident["Id"])
 
-            max_utime = int(time.time()) + (self.timeout *2)
+            max_utime = int(time.time()) + (self.timeout * 2)
 
             self.return_status["action"] = "Timed Out On Update"
 
             while int(time.time()) < max_utime:
                 changeset_info = self.cf_client.describe_change_set(ChangeSetName=changeset_ident["Id"])
 
                 execution_status = changeset_info["ExecutionStatus"]
@@ -397,8 +430,8 @@
             self.return_status["action"] = "CONFIRM OFF"
 
         elif pending_change == 0:
             # No Changes
             self.logger.info("{} : Stack Unchanged.".format(self.lname))
             self.return_status["action"] = "No Pending Changes"
 
-        return
+        return
```

### Comparing `cfn-ci-helper-2023.5.18.0/cfn_ci_helper.egg-info/PKG-INFO` & `cfn-ci-helper-2023.6.7.0/cfn_ci_helper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfn-ci-helper
-Version: 2023.5.18.0
+Version: 2023.6.7.0
 Summary: A Cloudformation CI Helper System
 Home-page: https://github.com/chalbersma/cfn-ci-helper
 Author: Chris Halbersma
 Author-email: chris@halbersma.us
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `cfn-ci-helper-2023.5.18.0/deploy_cf.py` & `cfn-ci-helper-2023.6.7.0/deploy_cf.py`

 * *Files identical despite different names*

### Comparing `cfn-ci-helper-2023.5.18.0/setup.cfg` & `cfn-ci-helper-2023.6.7.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cfn-ci-helper
-version = 2023.05.18.0
+version = 2023.06.07.0
 author = Chris Halbersma
 author_email = chris@halbersma.us
 description = A Cloudformation CI Helper System
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/chalbersma/cfn-ci-helper
 classifiers =
```

