# Comparing `tmp/codeflare_sdk-0.4.3.tar.gz` & `tmp/codeflare_sdk-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeflare_sdk-0.4.3.tar", max compression
+gzip compressed data, was "codeflare_sdk-0.4.4.tar", max compression
```

## Comparing `codeflare_sdk-0.4.3.tar` & `codeflare_sdk-0.4.4.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0    11357 2022-11-22 00:48:43.906021 codeflare_sdk-0.4.3/LICENSE
--rw-r--r--   0        0        0     1852 2023-04-11 19:26:34.779878 codeflare_sdk-0.4.3/README.md
--rw-r--r--   0        0        0      728 2023-04-12 21:05:15.628402 codeflare_sdk-0.4.3/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-16 18:31:44.974735 codeflare_sdk-0.4.3/src/codeflare_sdk/__init__.py
--rw-r--r--   0        0        0        0 2022-11-16 19:42:48.730723 codeflare_sdk-0.4.3/src/codeflare_sdk/cluster/__init__.py
--rw-r--r--   0        0        0     4434 2023-04-11 19:26:34.787878 codeflare_sdk-0.4.3/src/codeflare_sdk/cluster/auth.py
--rw-r--r--   0        0        0    17834 2023-04-11 19:26:34.788878 codeflare_sdk-0.4.3/src/codeflare_sdk/cluster/cluster.py
--rw-r--r--   0        0        0     1706 2023-04-11 19:26:34.788878 codeflare_sdk-0.4.3/src/codeflare_sdk/cluster/config.py
--rw-r--r--   0        0        0     2141 2023-03-06 15:15:54.772713 codeflare_sdk-0.4.3/src/codeflare_sdk/cluster/model.py
--rw-r--r--   0        0        0        0 2023-03-27 14:54:38.071640 codeflare_sdk-0.4.3/src/codeflare_sdk/job/__init__.py
--rw-r--r--   0        0        0     6618 2023-04-11 19:26:34.788878 codeflare_sdk-0.4.3/src/codeflare_sdk/job/jobs.py
--rw-r--r--   0        0        0    10292 2022-11-16 18:31:44.978735 codeflare_sdk-0.4.3/src/codeflare_sdk/templates/aw-kuberay.yaml
--rw-r--r--   0        0        0     7782 2023-04-11 19:26:34.788878 codeflare_sdk-0.4.3/src/codeflare_sdk/templates/base-template.yaml
--rw-r--r--   0        0        0    10080 2023-04-12 21:01:30.412216 codeflare_sdk-0.4.3/src/codeflare_sdk/templates/new-template.yaml
--rw-r--r--   0        0        0        0 2022-11-16 19:42:58.205776 codeflare_sdk-0.4.3/src/codeflare_sdk/utils/__init__.py
--rwxr-xr-x   0        0        0    10830 2023-02-02 16:52:21.915294 codeflare_sdk-0.4.3/src/codeflare_sdk/utils/generate_yaml.py
--rw-r--r--   0        0        0     6778 2023-03-27 14:54:38.071640 codeflare_sdk-0.4.3/src/codeflare_sdk/utils/pretty_print.py
--rw-r--r--   0        0        0     2850 1970-01-01 00:00:00.000000 codeflare_sdk-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-06 14:48:51.492503 codeflare_sdk-0.4.4/LICENSE
+-rw-r--r--   0        0        0     3501 2023-06-08 11:59:02.916039 codeflare_sdk-0.4.4/README.md
+-rw-r--r--   0        0        0      826 2023-06-08 12:24:02.233819 codeflare_sdk-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-06 14:48:51.497258 codeflare_sdk-0.4.4/src/codeflare_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 14:48:51.497352 codeflare_sdk-0.4.4/src/codeflare_sdk/cluster/__init__.py
+-rw-r--r--   0        0        0     4434 2023-04-10 20:47:55.250729 codeflare_sdk-0.4.4/src/codeflare_sdk/cluster/auth.py
+-rw-r--r--   0        0        0     3931 2023-06-07 19:18:08.800687 codeflare_sdk-0.4.4/src/codeflare_sdk/cluster/awload.py
+-rw-r--r--   0        0        0    17847 2023-06-07 19:18:08.801280 codeflare_sdk-0.4.4/src/codeflare_sdk/cluster/cluster.py
+-rw-r--r--   0        0        0     1706 2023-04-07 18:58:14.108111 codeflare_sdk-0.4.4/src/codeflare_sdk/cluster/config.py
+-rw-r--r--   0        0        0     2141 2023-04-06 14:48:51.497790 codeflare_sdk-0.4.4/src/codeflare_sdk/cluster/model.py
+-rw-r--r--   0        0        0        0 2023-04-06 14:48:51.497880 codeflare_sdk-0.4.4/src/codeflare_sdk/job/__init__.py
+-rw-r--r--   0        0        0     6618 2023-05-11 16:55:51.327687 codeflare_sdk-0.4.4/src/codeflare_sdk/job/jobs.py
+-rw-r--r--   0        0        0    10292 2023-04-06 14:48:51.498140 codeflare_sdk-0.4.4/src/codeflare_sdk/templates/aw-kuberay.yaml
+-rw-r--r--   0        0        0     7782 2023-04-10 20:47:55.251043 codeflare_sdk-0.4.4/src/codeflare_sdk/templates/base-template.yaml
+-rw-r--r--   0        0        0    10080 2023-05-11 16:55:51.328009 codeflare_sdk-0.4.4/src/codeflare_sdk/templates/new-template.yaml
+-rw-r--r--   0        0        0        0 2023-04-06 14:48:51.498421 codeflare_sdk-0.4.4/src/codeflare_sdk/utils/__init__.py
+-rwxr-xr-x   0        0        0    10830 2023-04-06 14:48:51.498552 codeflare_sdk-0.4.4/src/codeflare_sdk/utils/generate_yaml.py
+-rw-r--r--   0        0        0     6778 2023-04-06 14:48:51.498650 codeflare_sdk-0.4.4/src/codeflare_sdk/utils/pretty_print.py
+-rw-r--r--   0        0        0     4499 1970-01-01 00:00:00.000000 codeflare_sdk-0.4.4/PKG-INFO
```

### Comparing `codeflare_sdk-0.4.3/LICENSE` & `codeflare_sdk-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.4.3/pyproject.toml` & `codeflare_sdk-0.4.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "codeflare-sdk"
-version = "0.4.3"
+version = "0.4.4"
 description = "Python SDK for codeflare client"
 
 license = "Apache-2.0"
 
 authors = [
     "Michael Clifford <mcliffor@redhat.com>",
     "Mustafa Eyceoz <meyceoz@redhat.com>",
@@ -22,7 +22,13 @@
 [tool.poetry.dependencies]
 python = "^3.7"
 openshift-client = "1.0.18"
 rich = "^12.5"
 ray = {version = "2.1.0", extras = ["default"]}
 kubernetes = "26.1.0"
 codeflare-torchx = "0.6.0.dev0"
+
+[tool.poetry.group.docs]
+optional = true
+
+[tool.poetry.group.docs.dependencies]
+pdoc3 = "0.10.0"
```

### Comparing `codeflare_sdk-0.4.3/src/codeflare_sdk/cluster/auth.py` & `codeflare_sdk-0.4.4/src/codeflare_sdk/cluster/auth.py`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.4.3/src/codeflare_sdk/cluster/cluster.py` & `codeflare_sdk-0.4.4/src/codeflare_sdk/cluster/cluster.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
             if (
                 'the server doesn\'t have a resource type "AppWrapper"' in error_msg
                 or "forbidden" in error_msg
                 or "Unauthorized" in error_msg
                 or "Missing or incomplete configuration" in error_msg
             ):
                 raise PermissionError(
-                    "Action not permitted, have you run cluster.up() yet?"
+                    "Action not permitted, have you run auth.login()/cluster.up() yet?"
                 )
             elif "not found" in error_msg:
                 print("Cluster not found, have you run cluster.up() yet?")
             else:
                 raise osp
 
     def status(
```

### Comparing `codeflare_sdk-0.4.3/src/codeflare_sdk/cluster/config.py` & `codeflare_sdk-0.4.4/src/codeflare_sdk/cluster/config.py`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.4.3/src/codeflare_sdk/cluster/model.py` & `codeflare_sdk-0.4.4/src/codeflare_sdk/cluster/model.py`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.4.3/src/codeflare_sdk/job/jobs.py` & `codeflare_sdk-0.4.4/src/codeflare_sdk/job/jobs.py`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.4.3/src/codeflare_sdk/templates/aw-kuberay.yaml` & `codeflare_sdk-0.4.4/src/codeflare_sdk/templates/aw-kuberay.yaml`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.4.3/src/codeflare_sdk/templates/base-template.yaml` & `codeflare_sdk-0.4.4/src/codeflare_sdk/templates/base-template.yaml`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.4.3/src/codeflare_sdk/templates/new-template.yaml` & `codeflare_sdk-0.4.4/src/codeflare_sdk/templates/new-template.yaml`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.4.3/src/codeflare_sdk/utils/generate_yaml.py` & `codeflare_sdk-0.4.4/src/codeflare_sdk/utils/generate_yaml.py`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.4.3/src/codeflare_sdk/utils/pretty_print.py` & `codeflare_sdk-0.4.4/src/codeflare_sdk/utils/pretty_print.py`

 * *Files identical despite different names*

