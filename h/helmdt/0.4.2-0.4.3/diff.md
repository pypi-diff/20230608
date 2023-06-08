# Comparing `tmp/helmdt-0.4.2.tar.gz` & `tmp/helmdt-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helmdt-0.4.2.tar", last modified: Thu Jun  8 19:01:30 2023, max compression
+gzip compressed data, was "helmdt-0.4.3.tar", last modified: Thu Jun  8 19:04:32 2023, max compression
```

## Comparing `helmdt-0.4.2.tar` & `helmdt-0.4.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 19:01:30.884782 helmdt-0.4.2/
--rw-rw-rw-   0        0        0     1091 2023-06-08 08:25:00.000000 helmdt-0.4.2/LICENSE
--rw-rw-rw-   0        0        0       34 2023-06-08 18:40:53.000000 helmdt-0.4.2/MANIFEST.in
--rw-rw-rw-   0        0        0     6907 2023-06-08 19:01:30.884782 helmdt-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     6509 2023-06-08 18:25:07.000000 helmdt-0.4.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 19:01:30.874783 helmdt-0.4.2/helmdt.egg-info/
--rw-rw-rw-   0        0        0     6907 2023-06-08 19:01:30.000000 helmdt-0.4.2/helmdt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2023-06-08 19:01:30.000000 helmdt-0.4.2/helmdt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 19:01:30.000000 helmdt-0.4.2/helmdt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-06-08 19:01:30.000000 helmdt-0.4.2/helmdt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       32 2023-06-08 19:01:30.000000 helmdt-0.4.2/helmdt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-08 19:01:30.000000 helmdt-0.4.2/helmdt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     8109 2023-06-08 19:00:35.000000 helmdt-0.4.2/helmdt.py
--rw-rw-rw-   0        0        0       34 2023-06-08 18:27:52.000000 helmdt-0.4.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-08 19:01:30.884782 helmdt-0.4.2/setup.cfg
--rw-rw-rw-   0        0        0      901 2023-06-08 19:01:00.000000 helmdt-0.4.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-08 19:01:30.882785 helmdt-0.4.2/utils/
--rw-rw-rw-   0        0        0        0 2023-06-08 18:58:50.000000 helmdt-0.4.2/utils/__init__.py
--rw-rw-rw-   0        0        0     1772 2023-06-08 16:25:45.000000 helmdt-0.4.2/utils/azure.py
--rw-rw-rw-   0        0        0     1434 2023-06-08 10:28:27.000000 helmdt-0.4.2/utils/colorc.py
--rw-rw-rw-   0        0        0     2613 2023-06-08 16:30:41.000000 helmdt-0.4.2/utils/depcheck.py
--rw-rw-rw-   0        0        0     1064 2023-06-08 11:40:58.000000 helmdt-0.4.2/utils/docker.py
--rw-rw-rw-   0        0        0     1100 2023-06-08 16:58:15.000000 helmdt-0.4.2/utils/helm.py
--rw-rw-rw-   0        0        0     1161 2023-06-08 16:51:54.000000 helmdt-0.4.2/utils/run.py
+drwxrwxrwx   0        0        0        0 2023-06-08 19:04:32.662353 helmdt-0.4.3/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 08:25:00.000000 helmdt-0.4.3/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-06-08 18:40:53.000000 helmdt-0.4.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     6907 2023-06-08 19:04:32.662353 helmdt-0.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6509 2023-06-08 18:25:07.000000 helmdt-0.4.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 19:04:32.621356 helmdt-0.4.3/helmdt.egg-info/
+-rw-rw-rw-   0        0        0     6907 2023-06-08 19:04:32.000000 helmdt-0.4.3/helmdt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2023-06-08 19:04:32.000000 helmdt-0.4.3/helmdt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 19:04:32.000000 helmdt-0.4.3/helmdt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-06-08 19:04:32.000000 helmdt-0.4.3/helmdt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       32 2023-06-08 19:04:32.000000 helmdt-0.4.3/helmdt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-08 19:04:32.000000 helmdt-0.4.3/helmdt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8116 2023-06-08 19:03:30.000000 helmdt-0.4.3/helmdt.py
+-rw-rw-rw-   0        0        0       34 2023-06-08 18:27:52.000000 helmdt-0.4.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 19:04:32.663355 helmdt-0.4.3/setup.cfg
+-rw-rw-rw-   0        0        0      901 2023-06-08 19:04:17.000000 helmdt-0.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 19:04:32.660356 helmdt-0.4.3/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-08 18:58:50.000000 helmdt-0.4.3/utils/__init__.py
+-rw-rw-rw-   0        0        0     1757 2023-06-08 19:03:45.000000 helmdt-0.4.3/utils/azure.py
+-rw-rw-rw-   0        0        0     1434 2023-06-08 10:28:27.000000 helmdt-0.4.3/utils/colorc.py
+-rw-rw-rw-   0        0        0     2605 2023-06-08 19:03:58.000000 helmdt-0.4.3/utils/depcheck.py
+-rw-rw-rw-   0        0        0     1044 2023-06-08 19:04:04.000000 helmdt-0.4.3/utils/docker.py
+-rw-rw-rw-   0        0        0     1085 2023-06-08 19:04:09.000000 helmdt-0.4.3/utils/helm.py
+-rw-rw-rw-   0        0        0     1156 2023-06-08 19:04:12.000000 helmdt-0.4.3/utils/run.py
```

### Comparing `helmdt-0.4.2/LICENSE` & `helmdt-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `helmdt-0.4.2/PKG-INFO` & `helmdt-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helmdt
-Version: 0.4.2
+Version: 0.4.3
 Summary: A HELM Deployment toolkit
 Home-page: https://github.com/toshiya14/helmdt
 Author: Akaishi Toshiya
 Author-email: Toshiya14@live.jp
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
```

### Comparing `helmdt-0.4.2/README.md` & `helmdt-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `helmdt-0.4.2/helmdt.egg-info/PKG-INFO` & `helmdt-0.4.3/helmdt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helmdt
-Version: 0.4.2
+Version: 0.4.3
 Summary: A HELM Deployment toolkit
 Home-page: https://github.com/toshiya14/helmdt
 Author: Akaishi Toshiya
 Author-email: Toshiya14@live.jp
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
```

### Comparing `helmdt-0.4.2/helmdt.py` & `helmdt-0.4.3/helmdt.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 import click
 import yaml
 import os
 import sys
 from InquirerPy import prompt, inquirer
 from pathlib import Path
 
-from profiles import (
+from .profiles import (
     HelmEnvironmentProfile,
     HelmPackageProfile,
     load_profile,
     DeploymentProfile,
 )
-from utils.run import run, run_get_output
-from utils.azure import link_aks
-from utils.colorc import cc
-from utils.depcheck import checkdep
-from utils.docker import build_docker_image, push_docker_image
-from utils.helm import apply_helm_package
+from .utils.run import run, run_get_output
+from .utils.azure import link_aks
+from .utils.colorc import cc
+from .utils.depcheck import checkdep
+from .utils.docker import build_docker_image, push_docker_image
+from .utils.helm import apply_helm_package
 
 
 class runtime:
     def __init__(
         self,
         profile_file: str = None,
         profile: DeploymentProfile = None,
```

### Comparing `helmdt-0.4.2/setup.py` & `helmdt-0.4.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.read()
 
 setup(
     name="helmdt",
-    version="0.4.2",
+    version="0.4.3",
     author="Akaishi Toshiya",
     author_email="Toshiya14@live.jp",
     license="MIT",
     description="A HELM Deployment toolkit",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/toshiya14/helmdt",
```

### Comparing `helmdt-0.4.2/utils/azure.py` & `helmdt-0.4.3/utils/azure.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import subprocess
 import sys
 import functools
-from utils.colorc import cc as colorc
-from utils.depcheck import checkdep
-from utils.run import run
+from .colorc import cc as colorc
+from .depcheck import checkdep
+from .run import run
 
 
 def login_az():
     checkdep(["az"])
     return run("az login").returncode == 0
```

### Comparing `helmdt-0.4.2/utils/colorc.py` & `helmdt-0.4.3/utils/colorc.py`

 * *Files identical despite different names*

### Comparing `helmdt-0.4.2/utils/depcheck.py` & `helmdt-0.4.3/utils/depcheck.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from reprint import output
-from utils.colorc import bcolors, cc
-from utils.run import run
 import subprocess
 import sys
 
+from .colorc import bcolors, cc
+from .run import run
+
 deps = [
     {
         "name": "docker",
         "checkcmd": "docker --version",
         "url": "https://docs.docker.com/engine/install/",
         "checked": False,
     },
```

### Comparing `helmdt-0.4.2/utils/docker.py` & `helmdt-0.4.3/utils/docker.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from utils.azure import login_acr
-from utils.depcheck import checkdep
-from utils.run import promised_run
-from utils.colorc import cc
+from .azure import login_acr
+from .depcheck import checkdep
+from .run import promised_run
+from .colorc import cc
 import sys
 import re
 
 re_remote_image = re.compile(r"^(.*?)\.azurecr\.io\/(.*)$")
 
 def build_docker_image(dockerfile: str, build_context: str, image_name: str, no_cache:bool = False):
     checkdep(["docker"])
```

### Comparing `helmdt-0.4.2/utils/helm.py` & `helmdt-0.4.3/utils/helm.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import subprocess
-from utils.azure import retry_with_login_az_acr
-from utils.depcheck import checkdep
-from utils.run import run, promised_run, run_get_output
+from .azure import retry_with_login_az_acr
+from .depcheck import checkdep
+from .run import run, promised_run, run_get_output
 
 
 def apply_helm_package(
     dpname: str, namespace: str, kubecontext: str, package: str, values: str, tag: str
 ):
     checkdep(["helm", "kubectl"])
```

### Comparing `helmdt-0.4.2/utils/run.py` & `helmdt-0.4.3/utils/run.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import subprocess
 import platform
 import sys
 
-from utils.colorc import cc
+from .colorc import cc
 
 
 def run(
     cmd: str, preferred_shell: list[str] = None, stderr=None, stdout=None, cwd=None
 ):
     ps = preferred_shell
```

