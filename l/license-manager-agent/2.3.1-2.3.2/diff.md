# Comparing `tmp/license_manager_agent-2.3.1.tar.gz` & `tmp/license_manager_agent-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "license_manager_agent-2.3.1.tar", max compression
+gzip compressed data, was "license_manager_agent-2.3.2.tar", max compression
```

## Comparing `license_manager_agent-2.3.1.tar` & `license_manager_agent-2.3.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0       23 2023-05-22 18:46:11.414982 license_manager_agent-2.3.1/README.rst
--rw-r--r--   0        0        0        0 2023-05-22 18:46:11.414982 license_manager_agent-2.3.1/lm_agent/__init__.py
--rw-r--r--   0        0        0    10818 2023-05-22 18:46:11.414982 license_manager_agent-2.3.1/lm_agent/backend_utils.py
--rw-r--r--   0        0        0     3473 2023-05-22 18:46:11.414982 license_manager_agent-2.3.1/lm_agent/config.py
--rw-r--r--   0        0        0     1048 2023-05-22 18:46:11.414982 license_manager_agent-2.3.1/lm_agent/exceptions.py
--rw-r--r--   0        0        0     4032 2023-05-22 18:46:11.414982 license_manager_agent-2.3.1/lm_agent/license_report.py
--rw-r--r--   0        0        0     2000 2023-05-22 18:46:11.414982 license_manager_agent-2.3.1/lm_agent/logs.py
--rw-r--r--   0        0        0        0 2023-05-22 18:46:11.414982 license_manager_agent-2.3.1/lm_agent/parsing/__init__.py
--rw-r--r--   0        0        0     1732 2023-05-22 18:46:11.414982 license_manager_agent-2.3.1/lm_agent/parsing/flexlm.py
--rw-r--r--   0        0        0     3537 2023-05-22 18:46:11.414982 license_manager_agent-2.3.1/lm_agent/parsing/lmx.py
--rw-r--r--   0        0        0     4416 2023-05-22 18:46:11.414982 license_manager_agent-2.3.1/lm_agent/parsing/lsdyna.py
--rw-r--r--   0        0        0     4758 2023-05-22 18:46:11.414982 license_manager_agent-2.3.1/lm_agent/parsing/olicense.py
--rw-r--r--   0        0        0     2197 2023-05-22 18:46:11.414982 license_manager_agent-2.3.1/lm_agent/parsing/rlm.py
--rwxr-xr-x   0        0        0     1048 2023-05-22 18:46:11.414982 license_manager_agent-2.3.1/lm_agent/reconcile.py
--rw-r--r--   0        0        0    10660 2023-05-22 18:46:11.414982 license_manager_agent-2.3.1/lm_agent/reconciliation.py
--rw-r--r--   0        0        0        0 2023-05-22 18:46:11.414982 license_manager_agent-2.3.1/lm_agent/server_interfaces/__init__.py
--rw-r--r--   0        0        0     2904 2023-05-22 18:46:11.414982 license_manager_agent-2.3.1/lm_agent/server_interfaces/flexlm.py
--rw-r--r--   0        0        0     1665 2023-05-22 18:46:11.414982 license_manager_agent-2.3.1/lm_agent/server_interfaces/license_server_interface.py
--rw-r--r--   0        0        0     2751 2023-05-22 18:46:11.418982 license_manager_agent-2.3.1/lm_agent/server_interfaces/lmx.py
--rw-r--r--   0        0        0     2727 2023-05-22 18:46:11.418982 license_manager_agent-2.3.1/lm_agent/server_interfaces/lsdyna.py
--rw-r--r--   0        0        0     2719 2023-05-22 18:46:11.418982 license_manager_agent-2.3.1/lm_agent/server_interfaces/olicense.py
--rw-r--r--   0        0        0     3739 2023-05-22 18:46:11.418982 license_manager_agent-2.3.1/lm_agent/server_interfaces/rlm.py
--rw-r--r--   0        0        0     1251 2023-05-22 18:46:11.418982 license_manager_agent-2.3.1/lm_agent/utils.py
--rw-r--r--   0        0        0        0 2023-05-22 18:46:11.418982 license_manager_agent-2.3.1/lm_agent/workload_managers/__init__.py
--rw-r--r--   0        0        0        0 2023-05-22 18:46:11.418982 license_manager_agent-2.3.1/lm_agent/workload_managers/slurm/__init__.py
--rw-r--r--   0        0        0     8361 2023-05-22 18:46:11.418982 license_manager_agent-2.3.1/lm_agent/workload_managers/slurm/cmd_utils.py
--rw-r--r--   0        0        0     1036 2023-05-22 18:46:11.418982 license_manager_agent-2.3.1/lm_agent/workload_managers/slurm/common.py
--rw-r--r--   0        0        0     3732 2023-05-22 18:46:11.418982 license_manager_agent-2.3.1/lm_agent/workload_managers/slurm/reservations.py
--rw-r--r--   0        0        0     1728 2023-05-22 18:46:11.418982 license_manager_agent-2.3.1/lm_agent/workload_managers/slurm/slurmctld_epilog.py
--rw-r--r--   0        0        0     3923 2023-05-22 18:46:11.418982 license_manager_agent-2.3.1/lm_agent/workload_managers/slurm/slurmctld_prolog.py
--rw-r--r--   0        0        0     2050 2023-05-22 18:46:11.418982 license_manager_agent-2.3.1/pyproject.toml
--rw-r--r--   0        0        0     1053 1970-01-01 00:00:00.000000 license_manager_agent-2.3.1/PKG-INFO
+-rw-r--r--   0        0        0       23 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/README.rst
+-rw-r--r--   0        0        0        0 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/__init__.py
+-rw-r--r--   0        0        0    10818 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/backend_utils.py
+-rw-r--r--   0        0        0     3473 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/config.py
+-rw-r--r--   0        0        0     1048 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/exceptions.py
+-rw-r--r--   0        0        0     4032 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/license_report.py
+-rw-r--r--   0        0        0     2000 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/logs.py
+-rw-r--r--   0        0        0        0 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/parsing/__init__.py
+-rw-r--r--   0        0        0     1732 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/parsing/flexlm.py
+-rw-r--r--   0        0        0     3537 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/parsing/lmx.py
+-rw-r--r--   0        0        0     4416 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/parsing/lsdyna.py
+-rw-r--r--   0        0        0     4758 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/parsing/olicense.py
+-rw-r--r--   0        0        0     2197 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/parsing/rlm.py
+-rwxr-xr-x   0        0        0     1048 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/reconcile.py
+-rw-r--r--   0        0        0    10660 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/reconciliation.py
+-rw-r--r--   0        0        0        0 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/server_interfaces/__init__.py
+-rw-r--r--   0        0        0     2904 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/server_interfaces/flexlm.py
+-rw-r--r--   0        0        0     1665 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/server_interfaces/license_server_interface.py
+-rw-r--r--   0        0        0     2751 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/server_interfaces/lmx.py
+-rw-r--r--   0        0        0     2727 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/server_interfaces/lsdyna.py
+-rw-r--r--   0        0        0     2719 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/server_interfaces/olicense.py
+-rw-r--r--   0        0        0     3739 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/server_interfaces/rlm.py
+-rw-r--r--   0        0        0     1251 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/utils.py
+-rw-r--r--   0        0        0        0 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/workload_managers/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/workload_managers/slurm/__init__.py
+-rw-r--r--   0        0        0     8376 2023-06-08 19:49:38.911070 license_manager_agent-2.3.2/lm_agent/workload_managers/slurm/cmd_utils.py
+-rw-r--r--   0        0        0     1036 2023-06-08 19:49:38.911070 license_manager_agent-2.3.2/lm_agent/workload_managers/slurm/common.py
+-rw-r--r--   0        0        0     3732 2023-06-08 19:49:38.911070 license_manager_agent-2.3.2/lm_agent/workload_managers/slurm/reservations.py
+-rw-r--r--   0        0        0     1728 2023-06-08 19:49:38.911070 license_manager_agent-2.3.2/lm_agent/workload_managers/slurm/slurmctld_epilog.py
+-rw-r--r--   0        0        0     3923 2023-06-08 19:49:38.911070 license_manager_agent-2.3.2/lm_agent/workload_managers/slurm/slurmctld_prolog.py
+-rw-r--r--   0        0        0     2050 2023-06-08 19:49:38.911070 license_manager_agent-2.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1053 1970-01-01 00:00:00.000000 license_manager_agent-2.3.2/PKG-INFO
```

### Comparing `license_manager_agent-2.3.1/lm_agent/backend_utils.py` & `license_manager_agent-2.3.2/lm_agent/backend_utils.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.1/lm_agent/config.py` & `license_manager_agent-2.3.2/lm_agent/config.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.1/lm_agent/exceptions.py` & `license_manager_agent-2.3.2/lm_agent/exceptions.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.1/lm_agent/license_report.py` & `license_manager_agent-2.3.2/lm_agent/license_report.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.1/lm_agent/logs.py` & `license_manager_agent-2.3.2/lm_agent/logs.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.1/lm_agent/parsing/flexlm.py` & `license_manager_agent-2.3.2/lm_agent/parsing/flexlm.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.1/lm_agent/parsing/lmx.py` & `license_manager_agent-2.3.2/lm_agent/parsing/lmx.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.1/lm_agent/parsing/lsdyna.py` & `license_manager_agent-2.3.2/lm_agent/parsing/lsdyna.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.1/lm_agent/parsing/olicense.py` & `license_manager_agent-2.3.2/lm_agent/parsing/olicense.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.1/lm_agent/parsing/rlm.py` & `license_manager_agent-2.3.2/lm_agent/parsing/rlm.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.1/lm_agent/reconcile.py` & `license_manager_agent-2.3.2/lm_agent/reconcile.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.1/lm_agent/reconciliation.py` & `license_manager_agent-2.3.2/lm_agent/reconciliation.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.1/lm_agent/server_interfaces/flexlm.py` & `license_manager_agent-2.3.2/lm_agent/server_interfaces/flexlm.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.1/lm_agent/server_interfaces/license_server_interface.py` & `license_manager_agent-2.3.2/lm_agent/server_interfaces/license_server_interface.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.1/lm_agent/server_interfaces/lmx.py` & `license_manager_agent-2.3.2/lm_agent/server_interfaces/lmx.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.1/lm_agent/server_interfaces/lsdyna.py` & `license_manager_agent-2.3.2/lm_agent/server_interfaces/lsdyna.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.1/lm_agent/server_interfaces/olicense.py` & `license_manager_agent-2.3.2/lm_agent/server_interfaces/olicense.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.1/lm_agent/server_interfaces/rlm.py` & `license_manager_agent-2.3.2/lm_agent/server_interfaces/rlm.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.1/lm_agent/utils.py` & `license_manager_agent-2.3.2/lm_agent/utils.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.1/lm_agent/workload_managers/slurm/cmd_utils.py` & `license_manager_agent-2.3.2/lm_agent/workload_managers/slurm/cmd_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         """
         Return the line after the matched product_feature line.
         """
         matched = False
         for line in scontrol_output.split("\n"):
             if matched:
                 return line
-            if len(re.findall(rf"({product_feature_server})", line)) > 0:
+            if re.fullmatch(rf"LicenseName={product_feature_server}", line) is not None:
                 matched = True
         return None
 
     # Get the scontrol output
     scontrol_output = await scontrol_show_lic()
 
     # Match the product_feature_server
```

### Comparing `license_manager_agent-2.3.1/lm_agent/workload_managers/slurm/common.py` & `license_manager_agent-2.3.2/lm_agent/workload_managers/slurm/common.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.1/lm_agent/workload_managers/slurm/reservations.py` & `license_manager_agent-2.3.2/lm_agent/workload_managers/slurm/reservations.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.1/lm_agent/workload_managers/slurm/slurmctld_epilog.py` & `license_manager_agent-2.3.2/lm_agent/workload_managers/slurm/slurmctld_epilog.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.1/lm_agent/workload_managers/slurm/slurmctld_prolog.py` & `license_manager_agent-2.3.2/lm_agent/workload_managers/slurm/slurmctld_prolog.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.1/pyproject.toml` & `license_manager_agent-2.3.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "license-manager-agent"
-version = "2.3.1"
+version = "2.3.2"
 description = "Provides an agent for interacting with license manager"
 authors = ["OmniVector Solutions <info@omnivector.solutions>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/omnivector-solutions/license-manager"
 documentation = "https://omnivector-solutions.github.io/license-manager/"
 packages = [{ include = "lm_agent" }]
```

### Comparing `license_manager_agent-2.3.1/PKG-INFO` & `license_manager_agent-2.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: license-manager-agent
-Version: 2.3.1
+Version: 2.3.2
 Summary: Provides an agent for interacting with license manager
 Home-page: https://github.com/omnivector-solutions/license-manager
 License: MIT
 Author: OmniVector Solutions
 Author-email: info@omnivector.solutions
 Requires-Python: >=3.8,<3.9
 Classifier: License :: OSI Approved :: MIT License
```

