# Comparing `tmp/pyjaws-0.1.4.tar.gz` & `tmp/pyjaws-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjaws-0.1.4.tar", last modified: Sun May 21 14:19:59 2023, max compression
+gzip compressed data, was "pyjaws-0.1.5.tar", last modified: Thu Jun  8 13:10:54 2023, max compression
```

## Comparing `pyjaws-0.1.4.tar` & `pyjaws-0.1.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:19:59.838109 pyjaws-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-05-21 14:19:59.838109 pyjaws-0.1.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:19:59.834108 pyjaws-0.1.4/pyjaws/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-21 14:19:48.000000 pyjaws-0.1.4/pyjaws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:19:59.834108 pyjaws-0.1.4/pyjaws/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 14:19:48.000000 pyjaws-0.1.4/pyjaws/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-05-21 14:19:48.000000 pyjaws-0.1.4/pyjaws/api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-21 14:19:48.000000 pyjaws-0.1.4/pyjaws/api/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-21 14:19:48.000000 pyjaws-0.1.4/pyjaws/api/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-21 14:19:48.000000 pyjaws-0.1.4/pyjaws/api/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:19:59.834108 pyjaws-0.1.4/pyjaws/api/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:19:59.834108 pyjaws-0.1.4/pyjaws/api/templates/macros/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-21 14:19:48.000000 pyjaws-0.1.4/pyjaws/api/templates/macros/cluster.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-21 14:19:48.000000 pyjaws-0.1.4/pyjaws/api/templates/macros/task.j2
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-21 14:19:48.000000 pyjaws-0.1.4/pyjaws/api/templates/workflow.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:19:59.838109 pyjaws-0.1.4/pyjaws/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 14:19:48.000000 pyjaws-0.1.4/pyjaws/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-21 14:19:48.000000 pyjaws-0.1.4/pyjaws/client/entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:19:59.834108 pyjaws-0.1.4/pyjaws.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-05-21 14:19:59.000000 pyjaws-0.1.4/pyjaws.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-21 14:19:59.000000 pyjaws-0.1.4/pyjaws.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 14:19:59.000000 pyjaws-0.1.4/pyjaws.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-21 14:19:59.000000 pyjaws-0.1.4/pyjaws.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-21 14:19:59.000000 pyjaws-0.1.4/pyjaws.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-21 14:19:59.000000 pyjaws-0.1.4/pyjaws.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-21 14:19:48.000000 pyjaws-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 14:19:59.838109 pyjaws-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-21 14:19:48.000000 pyjaws-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:10:54.957575 pyjaws-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-06-08 13:10:54.957575 pyjaws-0.1.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:10:54.953575 pyjaws-0.1.5/pyjaws/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-08 13:10:38.000000 pyjaws-0.1.5/pyjaws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:10:54.957575 pyjaws-0.1.5/pyjaws/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 13:10:38.000000 pyjaws-0.1.5/pyjaws/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7609 2023-06-08 13:10:38.000000 pyjaws-0.1.5/pyjaws/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-08 13:10:38.000000 pyjaws-0.1.5/pyjaws/api/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-08 13:10:38.000000 pyjaws-0.1.5/pyjaws/api/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-08 13:10:38.000000 pyjaws-0.1.5/pyjaws/api/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:10:54.957575 pyjaws-0.1.5/pyjaws/api/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:10:54.957575 pyjaws-0.1.5/pyjaws/api/templates/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-08 13:10:38.000000 pyjaws-0.1.5/pyjaws/api/templates/macros/cluster.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-08 13:10:38.000000 pyjaws-0.1.5/pyjaws/api/templates/macros/task.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-08 13:10:38.000000 pyjaws-0.1.5/pyjaws/api/templates/workflow.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:10:54.957575 pyjaws-0.1.5/pyjaws/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 13:10:38.000000 pyjaws-0.1.5/pyjaws/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-06-08 13:10:38.000000 pyjaws-0.1.5/pyjaws/client/entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:10:54.957575 pyjaws-0.1.5/pyjaws.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-06-08 13:10:54.000000 pyjaws-0.1.5/pyjaws.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-08 13:10:54.000000 pyjaws-0.1.5/pyjaws.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 13:10:54.000000 pyjaws-0.1.5/pyjaws.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-08 13:10:54.000000 pyjaws-0.1.5/pyjaws.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-08 13:10:54.000000 pyjaws-0.1.5/pyjaws.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 13:10:54.000000 pyjaws-0.1.5/pyjaws.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-08 13:10:38.000000 pyjaws-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 13:10:54.957575 pyjaws-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-08 13:10:38.000000 pyjaws-0.1.5/setup.py
```

### Comparing `pyjaws-0.1.4/PKG-INFO` & `pyjaws-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pyjaws
-Version: 0.1.4
+Version: 0.1.5
 Author: Rafael Pierre
 Description-Content-Type: text/markdown
 
 # PyJaws: A Pythonic Way to Define Databricks Jobs and Workflows
 
 <p align="center">
         <img src="https://raw.githubusercontent.com/rafaelpierre/pyjaws/main/img/pyjaws.png" class="align-center" />
     </a>
 </p>
 
 <hr />
 
-[![pypi](https://img.shields.io/badge/pypi-0.1.4-brightgreen?style=for-the-badge)](https://pypi.org/project/pyjaws/) ![black](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge) ![ruff](https://img.shields.io/badge/lint-ruff-gold?style=for-the-badge) ![cov](https://raw.githubusercontent.com/rafaelpierre/pyjaws/main/img/coverage.svg) ![databricks](https://img.shields.io/badge/Databricks-FF3621.svg?style=for-the-badge&logo=Databricks&logoColor=white) ![Jinja](https://img.shields.io/badge/jinja-white.svg?style=for-the-badge&logo=jinja&logoColor=black) ![downloads](https://img.shields.io/pypi/dm/pyjaws?style=for-the-badge)
+[![pypi](https://img.shields.io/badge/pypi-0.1.5-brightgreen?style=for-the-badge)](https://pypi.org/project/pyjaws/) ![black](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge) ![ruff](https://img.shields.io/badge/lint-ruff-gold?style=for-the-badge) ![cov](https://raw.githubusercontent.com/rafaelpierre/pyjaws/main/img/coverage.svg) ![databricks](https://img.shields.io/badge/Databricks-FF3621.svg?style=for-the-badge&logo=Databricks&logoColor=white) ![Jinja](https://img.shields.io/badge/jinja-white.svg?style=for-the-badge&logo=jinja&logoColor=black) ![downloads](https://img.shields.io/pypi/dm/pyjaws?style=for-the-badge)
 
 <hr />
 
 * **PyJaws** enables declaring [Databricks Jobs and Workflows](https://docs.databricks.com/workflows/index.html) as Python code, allowing for:
   * Code Linting
   * Formatting
   * Parameter Validation
```

### Comparing `pyjaws-0.1.4/pyjaws/api/base.py` & `pyjaws-0.1.5/pyjaws/api/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-"""Base class for Husk Databricks Jobs & Workflows."""
+"""Base class for PyJaws Databricks Jobs & Workflows."""
 
 from __future__ import annotations
-import jinja2
-import logging
+
 import json
-from json.decoder import JSONDecodeError
-import rapidjson
+import logging
+import os
 from datetime import datetime
-from matplotlib import pyplot as plt
-
+from json.decoder import JSONDecodeError
+from threading import Lock
 from typing import List, Optional
-from pydantic import BaseModel
-import os
-import networkx as nx
 
 import git
+import jinja2
+import networkx as nx
+import rapidjson
+from matplotlib import pyplot as plt
+from pydantic import BaseModel
 
 from pyjaws import __version__
 from pyjaws.api.runtime import Runtime
 
-
 BASE_PATH = os.path.dirname(__file__)
-WHEEL_NAME = f"husk-{__version__}-py3-none-any.whl"
-WHEEL_REMOTE_PATH = f"dbfs:/FileStore/husk/{WHEEL_NAME}/{WHEEL_NAME}"
 
 
 class Cluster(BaseModel):
     job_cluster_key: str
     spark_version: Runtime
     num_workers: int
     node_type_id: Optional[str] = None
     autoscale: Optional[bool] = None
     instance_pool_id: Optional[str] = None
     runtime_engine: Optional[str] = None
     cluster_log_conf: Optional[dict] = None
+    __cluster: List[Cluster] = []  # mutable list to store current instance
+    __lock: Lock = Lock()  # to prevent race conditions
 
     def __init__(self, **kwargs):
         """
         Creates a cluster object.
         Params:
             job_cluster_key (str): Job Cluster identifying key.\n
             spark_version (pyjaws.api.base.Cluster): Spark Cluster Runtime.\n
@@ -51,18 +51,32 @@
         """
         super().__init__(**kwargs)
 
     def __str__(self):
         return self.job_cluster_key
 
     def __enter__(self) -> Cluster:
+        """Injects cluster instance into tasks created within context manger syntax."""
+        if self.__cluster:
+            raise Exception("Nested clusters are not supported!!")
+        self.__lock.acquire()
+        self.__cluster.append(self)
         return self
 
     def __exit__(self, *args):
-        pass
+        self.__cluster.pop()
+        self.__lock.release()
+
+    @classmethod
+    def _get_cluster(cls) -> Cluster:
+        """A helper method to return the cluster instance."""
+        if cls.__cluster:
+            return cls.__cluster[-1]
+        else:
+            raise Exception("_get_cluster cannot be called outside of with clause!!")
 
     @property
     def cluster_log_conf_str(self) -> str:
         return json.dumps(self.cluster_log_conf)
 
 
 class BaseTask(BaseModel):
@@ -71,20 +85,22 @@
     Params:
         key: Task key.
         cluster: Cluster object for running the task.
         libraries: List of Python libraries to be installed.
     """
 
     key: str
-    cluster: Cluster
+    cluster: Optional[Cluster] = None
     dependencies: Optional[List[BaseTask]] = []
     libraries: Optional[List[dict]] = None
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
+        if not self.cluster and Cluster._get_cluster():
+            self.cluster = Cluster._get_cluster()
 
     def __str__(self):
         return self.key
 
     def set_relatives(self, downstream, task_or_task_list):
         if isinstance(task_or_task_list, list):
             for task in task_or_task_list:
```

### Comparing `pyjaws-0.1.4/pyjaws/api/jobs.py` & `pyjaws-0.1.5/pyjaws/api/jobs.py`

 * *Files identical despite different names*

### Comparing `pyjaws-0.1.4/pyjaws/api/tasks.py` & `pyjaws-0.1.5/pyjaws/api/tasks.py`

 * *Files identical despite different names*

### Comparing `pyjaws-0.1.4/pyjaws/api/templates/macros/cluster.j2` & `pyjaws-0.1.5/pyjaws/api/templates/macros/cluster.j2`

 * *Files identical despite different names*

### Comparing `pyjaws-0.1.4/pyjaws/api/templates/macros/task.j2` & `pyjaws-0.1.5/pyjaws/api/templates/macros/task.j2`

 * *Files identical despite different names*

### Comparing `pyjaws-0.1.4/pyjaws/api/templates/workflow.j2` & `pyjaws-0.1.5/pyjaws/api/templates/workflow.j2`

 * *Files identical despite different names*

### Comparing `pyjaws-0.1.4/pyjaws/client/entrypoint.py` & `pyjaws-0.1.5/pyjaws/client/entrypoint.py`

 * *Files identical despite different names*

### Comparing `pyjaws-0.1.4/pyjaws.egg-info/PKG-INFO` & `pyjaws-0.1.5/pyjaws.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pyjaws
-Version: 0.1.4
+Version: 0.1.5
 Author: Rafael Pierre
 Description-Content-Type: text/markdown
 
 # PyJaws: A Pythonic Way to Define Databricks Jobs and Workflows
 
 <p align="center">
         <img src="https://raw.githubusercontent.com/rafaelpierre/pyjaws/main/img/pyjaws.png" class="align-center" />
     </a>
 </p>
 
 <hr />
 
-[![pypi](https://img.shields.io/badge/pypi-0.1.4-brightgreen?style=for-the-badge)](https://pypi.org/project/pyjaws/) ![black](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge) ![ruff](https://img.shields.io/badge/lint-ruff-gold?style=for-the-badge) ![cov](https://raw.githubusercontent.com/rafaelpierre/pyjaws/main/img/coverage.svg) ![databricks](https://img.shields.io/badge/Databricks-FF3621.svg?style=for-the-badge&logo=Databricks&logoColor=white) ![Jinja](https://img.shields.io/badge/jinja-white.svg?style=for-the-badge&logo=jinja&logoColor=black) ![downloads](https://img.shields.io/pypi/dm/pyjaws?style=for-the-badge)
+[![pypi](https://img.shields.io/badge/pypi-0.1.5-brightgreen?style=for-the-badge)](https://pypi.org/project/pyjaws/) ![black](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge) ![ruff](https://img.shields.io/badge/lint-ruff-gold?style=for-the-badge) ![cov](https://raw.githubusercontent.com/rafaelpierre/pyjaws/main/img/coverage.svg) ![databricks](https://img.shields.io/badge/Databricks-FF3621.svg?style=for-the-badge&logo=Databricks&logoColor=white) ![Jinja](https://img.shields.io/badge/jinja-white.svg?style=for-the-badge&logo=jinja&logoColor=black) ![downloads](https://img.shields.io/pypi/dm/pyjaws?style=for-the-badge)
 
 <hr />
 
 * **PyJaws** enables declaring [Databricks Jobs and Workflows](https://docs.databricks.com/workflows/index.html) as Python code, allowing for:
   * Code Linting
   * Formatting
   * Parameter Validation
```

### Comparing `pyjaws-0.1.4/pyproject.toml` & `pyjaws-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyjaws-0.1.4/setup.py` & `pyjaws-0.1.5/setup.py`

 * *Files identical despite different names*

