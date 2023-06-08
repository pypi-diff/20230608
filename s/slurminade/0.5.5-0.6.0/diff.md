# Comparing `tmp/slurminade-0.5.5.tar.gz` & `tmp/slurminade-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slurminade-0.5.5.tar", last modified: Tue Apr 25 18:41:02 2023, max compression
+gzip compressed data, was "slurminade-0.6.0.tar", last modified: Thu Jun  8 19:44:50 2023, max compression
```

## Comparing `slurminade-0.5.5.tar` & `slurminade-0.6.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:41:02.638523 slurminade-0.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-25 18:40:57.000000 slurminade-0.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8136 2023-04-25 18:41:02.638523 slurminade-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7654 2023-04-25 18:40:57.000000 slurminade-0.5.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-25 18:40:57.000000 slurminade-0.5.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 18:41:02.638523 slurminade-0.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-25 18:40:57.000000 slurminade-0.5.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:41:02.634523 slurminade-0.5.5/slurminade/
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-25 18:40:57.000000 slurminade-0.5.5/slurminade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-04-25 18:40:57.000000 slurminade-0.5.5/slurminade/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-25 18:40:57.000000 slurminade-0.5.5/slurminade/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    12820 2023-04-25 18:40:57.000000 slurminade-0.5.5/slurminade/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-25 18:40:57.000000 slurminade-0.5.5/slurminade/execute.py
--rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-04-25 18:40:57.000000 slurminade-0.5.5/slurminade/function.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-04-25 18:40:57.000000 slurminade-0.5.5/slurminade/function_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-25 18:40:57.000000 slurminade-0.5.5/slurminade/guard.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-25 18:40:57.000000 slurminade-0.5.5/slurminade/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:41:02.638523 slurminade-0.5.5/slurminade.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8136 2023-04-25 18:41:02.000000 slurminade-0.5.5/slurminade.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-25 18:41:02.000000 slurminade-0.5.5/slurminade.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 18:41:02.000000 slurminade-0.5.5/slurminade.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 18:41:02.000000 slurminade-0.5.5/slurminade.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-25 18:41:02.000000 slurminade-0.5.5/slurminade.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-25 18:41:02.000000 slurminade-0.5.5/slurminade.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:44:50.183711 slurminade-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-08 19:44:44.000000 slurminade-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-06-08 19:44:50.183711 slurminade-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-06-08 19:44:44.000000 slurminade-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-08 19:44:44.000000 slurminade-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 19:44:50.183711 slurminade-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-08 19:44:44.000000 slurminade-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:44:50.183711 slurminade-0.6.0/slurminade/
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-06-08 19:44:44.000000 slurminade-0.6.0/slurminade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-06-08 19:44:44.000000 slurminade-0.6.0/slurminade/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-08 19:44:44.000000 slurminade-0.6.0/slurminade/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13353 2023-06-08 19:44:44.000000 slurminade-0.6.0/slurminade/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-06-08 19:44:44.000000 slurminade-0.6.0/slurminade/execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-06-08 19:44:44.000000 slurminade-0.6.0/slurminade/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-06-08 19:44:44.000000 slurminade-0.6.0/slurminade/function_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-08 19:44:44.000000 slurminade-0.6.0/slurminade/guard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-08 19:44:44.000000 slurminade-0.6.0/slurminade/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:44:50.183711 slurminade-0.6.0/slurminade.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-06-08 19:44:50.000000 slurminade-0.6.0/slurminade.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-08 19:44:50.000000 slurminade-0.6.0/slurminade.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 19:44:50.000000 slurminade-0.6.0/slurminade.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 19:44:50.000000 slurminade-0.6.0/slurminade.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-08 19:44:50.000000 slurminade-0.6.0/slurminade.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-08 19:44:50.000000 slurminade-0.6.0/slurminade.egg-info/top_level.txt
```

### Comparing `slurminade-0.5.5/LICENSE` & `slurminade-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `slurminade-0.5.5/PKG-INFO` & `slurminade-0.6.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: slurminade
-Version: 0.5.5
-Summary: A decorator-based slurm runner
-Home-page: https://github.com/d-krupke/slurminade
-Author: Dominik Krupke
-Author-email: krupke@ibr.cs.tu-bs.de
-License: MIT
-Keywords: slurm
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # slurminade
 
 *slurminade* makes using the workload manager [slurm](https://slurm.schedmd.com/documentation.html) with Python beautiful.
 It is based on [simple_slurm](https://github.com/amq92/simple_slurm), but instead of just allowing to comfortably execute shell commands in slurm, it allows to directly distribute Python-functions.
 A function decorated with `@slurminade.slurmify(partition="alg")` will automatically be executed by a node of the partition `alg` by just calling `.distribute(yes_also_args_are_allowed)`.
 The general idea is that the corresponding Python-code exists on both machines, thus, the slurm-node can also call the functions of the original code if you tell if which one and what arguments to use.
 This is similar to [celery](https://github.com/celery/celery) but you do not need to install anything, just make sure the same Python-environment is available the nodes (usually the case in a proper slurm setup).
@@ -212,21 +195,21 @@
 - function.py: Contains the code for making a function slurm-compatible.
 - function_map.py: Saves all the slurmified functions.
 - guard.py: Contains code to prevent you accidentally DDoSing your infrastructure.
 - options.py: Contains a simple data structure to save slurm options.
 
 ## Changes
 
+* 0.6.0: Autmatic naming of tasks.
 * 0.5.5: Fixing bug guard bug in subprocess dispatcher.
 * 0.5.4: Dispatched function calls that are too long for the command line now use a temporary file instead.
 * 0.5.3: Fixed a bug that caused the dispatch limit to have no effect.
 * 0.5.2: Added pyproject.toml for PEP compliance
 * 0.5.1: `Batch` will now flush on delete, in case you forgot.
 * 0.5.0:
   * Functions now have a `wait_for`-option and return job ids. 
   * Braking changes: Batches have a new API.
     * `add` is no longer needed.
     * `AutoBatch` is now called `Batch`.
   * Fundamental code changes under the hood.
 * <0.5.0:
-  * Lots of experiments on finding the right interface.
-
+  * Lots of experiments on finding the right interface.
```

### Comparing `slurminade-0.5.5/README.md` & `slurminade-0.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: slurminade
+Version: 0.6.0
+Summary: A decorator-based slurm runner
+Home-page: https://github.com/d-krupke/slurminade
+Author: Dominik Krupke
+Author-email: krupke@ibr.cs.tu-bs.de
+License: MIT
+Keywords: slurm
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # slurminade
 
 *slurminade* makes using the workload manager [slurm](https://slurm.schedmd.com/documentation.html) with Python beautiful.
 It is based on [simple_slurm](https://github.com/amq92/simple_slurm), but instead of just allowing to comfortably execute shell commands in slurm, it allows to directly distribute Python-functions.
 A function decorated with `@slurminade.slurmify(partition="alg")` will automatically be executed by a node of the partition `alg` by just calling `.distribute(yes_also_args_are_allowed)`.
 The general idea is that the corresponding Python-code exists on both machines, thus, the slurm-node can also call the functions of the original code if you tell if which one and what arguments to use.
 This is similar to [celery](https://github.com/celery/celery) but you do not need to install anything, just make sure the same Python-environment is available the nodes (usually the case in a proper slurm setup).
@@ -195,20 +212,22 @@
 - function.py: Contains the code for making a function slurm-compatible.
 - function_map.py: Saves all the slurmified functions.
 - guard.py: Contains code to prevent you accidentally DDoSing your infrastructure.
 - options.py: Contains a simple data structure to save slurm options.
 
 ## Changes
 
+* 0.6.0: Autmatic naming of tasks.
 * 0.5.5: Fixing bug guard bug in subprocess dispatcher.
 * 0.5.4: Dispatched function calls that are too long for the command line now use a temporary file instead.
 * 0.5.3: Fixed a bug that caused the dispatch limit to have no effect.
 * 0.5.2: Added pyproject.toml for PEP compliance
 * 0.5.1: `Batch` will now flush on delete, in case you forgot.
 * 0.5.0:
   * Functions now have a `wait_for`-option and return job ids. 
   * Braking changes: Batches have a new API.
     * `add` is no longer needed.
     * `AutoBatch` is now called `Batch`.
   * Fundamental code changes under the hood.
 * <0.5.0:
-  * Lots of experiments on finding the right interface.
+  * Lots of experiments on finding the right interface.
+
```

### Comparing `slurminade-0.5.5/setup.py` & `slurminade-0.6.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open("README.md") as f:
         return f.read()
 
 
 setup(
     name="slurminade",
-    version="0.5.5",
+    version="0.6.0",
     description="A decorator-based slurm runner",
     long_description=readme(),
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
```

### Comparing `slurminade-0.5.5/slurminade/__init__.py` & `slurminade-0.6.0/slurminade/__init__.py`

 * *Files identical despite different names*

### Comparing `slurminade-0.5.5/slurminade/batch.py` & `slurminade-0.6.0/slurminade/batch.py`

 * *Files identical despite different names*

### Comparing `slurminade-0.5.5/slurminade/conf.py` & `slurminade-0.6.0/slurminade/conf.py`

 * *Files identical despite different names*

### Comparing `slurminade-0.5.5/slurminade/dispatcher.py` & `slurminade-0.6.0/slurminade/dispatcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 import subprocess
 import sys
 import typing
 from tempfile import mkstemp
 
 import simple_slurm
 
-from slurminade.conf import _get_conf
-from slurminade.function_map import FunctionMap, get_entry_point
-from slurminade.guard import dispatch_guard
-from slurminade.options import SlurmOptions
+from .conf import _get_conf
+from .function_map import FunctionMap, get_entry_point
+from .guard import dispatch_guard
+from .options import SlurmOptions
 
 
 # MAX_ARG_STRLEN on a Linux system with PAGE_SIZE 4096 is 131072
 DEFAULT_MAX_ARG_LENGTH = 100000
 
 
 class FunctionCall:
@@ -181,19 +181,33 @@
             raise RuntimeError("Slurm could not be found.")
         self.max_arg_length = DEFAULT_MAX_ARG_LENGTH
 
     def _create_slurm_api(self, special_slurm_opts):
         conf = _get_conf(special_slurm_opts)
         slurm = simple_slurm.Slurm(**conf)
         return slurm
+    
+    def _task_name(funcs: typing.List[FunctionCall]) -> str:
+        func_names = list(set(FunctionMap.get_readable_name(f.func_id) for f in funcs))
+        if len(funcs) == 1:
+            return f"slurminade: {func_names[0]}"
+        else:
+            if len(func_names)<=3:
+                return f"slurminade[batch]: {func_names}"
+            else:
+                return f"slurminade[batch]: {func_names[:3]}..."
+        
 
     def _dispatch(
         self, funcs: typing.Iterable[FunctionCall], options: SlurmOptions
     ) -> int:
         dispatch_guard()
+        if "task_name" not in options:
+            funcs = list(funcs)
+            options = {"task_name": self._task_name(funcs), **options}
         slurm = self._create_slurm_api(options)
         command = create_slurminade_command(funcs, self.max_arg_length)
         return slurm.sbatch(command)
 
     def sbatch(self, command: str, conf: dict = None, simple_slurm_kwargs: dict = None):
         dispatch_guard()
         conf = _get_conf(conf)
```

### Comparing `slurminade-0.5.5/slurminade/execute.py` & `slurminade-0.6.0/slurminade/execute.py`

 * *Files identical despite different names*

### Comparing `slurminade-0.5.5/slurminade/function.py` & `slurminade-0.6.0/slurminade/function.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,17 @@
         :return: Job id. Not necessarily valid (usually -1 in this case).
         """
         self._check(args, kwargs)
         guard_recursive_distribution()
         return dispatch(
             [FunctionCall(self.func_id, args, kwargs)], self.special_slurm_opts
         )
+    
+    def __str__(self) -> str:
+        return self.func.__name__
 
     @staticmethod
     def call(func_id, *args, **kwargs):
         return FunctionMap.call(func_id, args, kwargs)
 
 
 def slurmify(f=None, **args) -> typing.Callable[[typing.Callable], SlurmFunction]:
```

### Comparing `slurminade-0.5.5/slurminade/function_map.py` & `slurminade-0.6.0/slurminade/function_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,19 @@
         if file == "<string>":  # on the slurm node, the functions in the entry point
             # are named `<string>`.
             if not FunctionMap.entry_point:
                 raise RuntimeError("No entry point known.")
             file = FunctionMap.entry_point
         path = os.path.normpath(os.path.abspath(file))
         return f"{path}:{func.__name__}"
+    
+    @staticmethod
+    def get_readable_name(func_id: str) -> str:
+        return func_id.split(":")[-1]
+
 
     @staticmethod
     def check_compatibility(func: typing.Callable):
         """
         Throw if the function cannot be assigned an id.
         :param func: The function to be checked.
         :return: None
```

### Comparing `slurminade-0.5.5/slurminade/guard.py` & `slurminade-0.6.0/slurminade/guard.py`

 * *Files identical despite different names*

### Comparing `slurminade-0.5.5/slurminade/options.py` & `slurminade-0.6.0/slurminade/options.py`

 * *Files identical despite different names*

### Comparing `slurminade-0.5.5/slurminade.egg-info/PKG-INFO` & `slurminade-0.6.0/slurminade.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurminade
-Version: 0.5.5
+Version: 0.6.0
 Summary: A decorator-based slurm runner
 Home-page: https://github.com/d-krupke/slurminade
 Author: Dominik Krupke
 Author-email: krupke@ibr.cs.tu-bs.de
 License: MIT
 Keywords: slurm
 Platform: UNKNOWN
@@ -212,14 +212,15 @@
 - function.py: Contains the code for making a function slurm-compatible.
 - function_map.py: Saves all the slurmified functions.
 - guard.py: Contains code to prevent you accidentally DDoSing your infrastructure.
 - options.py: Contains a simple data structure to save slurm options.
 
 ## Changes
 
+* 0.6.0: Autmatic naming of tasks.
 * 0.5.5: Fixing bug guard bug in subprocess dispatcher.
 * 0.5.4: Dispatched function calls that are too long for the command line now use a temporary file instead.
 * 0.5.3: Fixed a bug that caused the dispatch limit to have no effect.
 * 0.5.2: Added pyproject.toml for PEP compliance
 * 0.5.1: `Batch` will now flush on delete, in case you forgot.
 * 0.5.0:
   * Functions now have a `wait_for`-option and return job ids.
```

