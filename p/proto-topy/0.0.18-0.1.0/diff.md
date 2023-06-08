# Comparing `tmp/proto-topy-0.0.18.tar.gz` & `tmp/proto-topy-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proto-topy-0.0.18.tar", last modified: Thu Nov 17 18:49:29 2022, max compression
+gzip compressed data, was "proto-topy-0.1.0.tar", last modified: Thu Jun  8 16:27:47 2023, max compression
```

## Comparing `proto-topy-0.0.18.tar` & `proto-topy-0.1.0.tar`

### file list

```diff
@@ -1,37 +1,33 @@
-drwxr-xr-x   0 decitre    (501) staff       (20)        0 2022-11-17 18:49:29.164267 proto-topy-0.0.18/
--rw-r--r--   0 decitre    (501) staff       (20)      194 2022-11-17 16:49:02.000000 proto-topy-0.0.18/.bumpversion.cfg
--rw-r--r--   0 decitre    (501) staff       (20)      178 2022-04-10 09:04:13.000000 proto-topy-0.0.18/.coveragerc
--rw-r--r--   0 decitre    (501) staff       (20)      636 2022-04-10 09:04:13.000000 proto-topy-0.0.18/.pre-commit-config.yaml
--rw-r--r--   0 decitre    (501) staff       (20)     1204 2022-04-12 06:44:18.000000 proto-topy-0.0.18/LICENSE
--rw-r--r--   0 decitre    (501) staff       (20)      313 2022-11-17 16:44:09.000000 proto-topy-0.0.18/MANIFEST.in
--rw-r--r--   0 decitre    (501) staff       (20)     2481 2022-11-17 18:49:29.164483 proto-topy-0.0.18/PKG-INFO
--rw-r--r--   0 decitre    (501) staff       (20)     1557 2022-11-17 16:37:43.000000 proto-topy-0.0.18/README.md
-drwxr-xr-x   0 decitre    (501) staff       (20)        0 2022-11-17 18:49:29.153773 proto-topy-0.0.18/ci/
--rwxr-xr-x   0 decitre    (501) staff       (20)     3063 2022-04-10 09:04:13.000000 proto-topy-0.0.18/ci/bootstrap.py
--rw-r--r--   0 decitre    (501) staff       (20)       66 2022-04-10 09:04:13.000000 proto-topy-0.0.18/ci/requirements.txt
-drwxr-xr-x   0 decitre    (501) staff       (20)        0 2022-11-17 18:49:29.144350 proto-topy-0.0.18/ci/templates/
-drwxr-xr-x   0 decitre    (501) staff       (20)        0 2022-11-17 18:49:29.144438 proto-topy-0.0.18/ci/templates/.github/
-drwxr-xr-x   0 decitre    (501) staff       (20)        0 2022-11-17 18:49:29.154432 proto-topy-0.0.18/ci/templates/.github/workflows/
--rw-r--r--   0 decitre    (501) staff       (20)     2001 2022-04-10 09:04:13.000000 proto-topy-0.0.18/ci/templates/.github/workflows/github-actions.yml
--rw-r--r--   0 decitre    (501) staff       (20)      159 2022-04-10 09:28:09.000000 proto-topy-0.0.18/pyproject.toml
--rw-r--r--   0 decitre    (501) staff       (20)        8 2022-04-10 17:23:50.000000 proto-topy-0.0.18/requirements.txt
--rw-r--r--   0 decitre    (501) staff       (20)       15 2022-04-13 05:27:53.000000 proto-topy-0.0.18/requirements_test.txt
--rw-r--r--   0 decitre    (501) staff       (20)      670 2022-11-17 18:49:29.165470 proto-topy-0.0.18/setup.cfg
--rwxr-xr-x   0 decitre    (501) staff       (20)     3668 2022-11-17 18:47:33.000000 proto-topy-0.0.18/setup.py
-drwxr-xr-x   0 decitre    (501) staff       (20)        0 2022-11-17 18:49:29.144827 proto-topy-0.0.18/src/
-drwxr-xr-x   0 decitre    (501) staff       (20)        0 2022-11-17 18:49:29.155429 proto-topy-0.0.18/src/proto_topy/
--rw-r--r--   0 decitre    (501) staff       (20)       61 2022-11-17 18:35:33.000000 proto-topy-0.0.18/src/proto_topy/__init__.py
--rw-r--r--   0 decitre    (501) staff       (20)     9195 2022-11-17 18:23:27.000000 proto-topy-0.0.18/src/proto_topy/entities.py
-drwxr-xr-x   0 decitre    (501) staff       (20)        0 2022-11-17 18:49:29.160907 proto-topy-0.0.18/src/proto_topy.egg-info/
--rw-r--r--   0 decitre    (501) staff       (20)     2481 2022-11-17 18:49:29.000000 proto-topy-0.0.18/src/proto_topy.egg-info/PKG-INFO
--rw-r--r--   0 decitre    (501) staff       (20)      623 2022-11-17 18:49:29.000000 proto-topy-0.0.18/src/proto_topy.egg-info/SOURCES.txt
--rw-r--r--   0 decitre    (501) staff       (20)        1 2022-11-17 18:49:29.000000 proto-topy-0.0.18/src/proto_topy.egg-info/dependency_links.txt
--rw-r--r--   0 decitre    (501) staff       (20)        1 2022-04-10 14:48:33.000000 proto-topy-0.0.18/src/proto_topy.egg-info/not-zip-safe
--rw-r--r--   0 decitre    (501) staff       (20)       38 2022-11-17 18:49:29.000000 proto-topy-0.0.18/src/proto_topy.egg-info/requires.txt
--rw-r--r--   0 decitre    (501) staff       (20)       11 2022-11-17 18:49:29.000000 proto-topy-0.0.18/src/proto_topy.egg-info/top_level.txt
-drwxr-xr-x   0 decitre    (501) staff       (20)        0 2022-11-17 18:49:29.163493 proto-topy-0.0.18/tests/
--rw-r--r--   0 decitre    (501) staff       (20)    36296 2022-04-24 13:05:49.000000 proto-topy-0.0.18/tests/_test_proto_topy_intern.py
--rw-r--r--   0 decitre    (501) staff       (20)      481 2022-04-13 06:06:09.000000 proto-topy-0.0.18/tests/artifact.fds
--rw-r--r--   0 decitre    (501) staff       (20)        0 2022-04-12 05:32:10.000000 proto-topy-0.0.18/tests/test.proto
--rw-r--r--   0 decitre    (501) staff       (20)     6644 2022-11-17 18:16:13.000000 proto-topy-0.0.18/tests/test_proto_topy.py
--rw-r--r--   0 decitre    (501) staff       (20)     1347 2022-04-13 11:07:38.000000 proto-topy-0.0.18/tox.ini
+drwxr-xr-x   0 decitre    (501) staff       (20)        0 2023-06-08 16:27:47.959382 proto-topy-0.1.0/
+-rw-r--r--   0 decitre    (501) staff       (20)      178 2022-04-10 09:04:13.000000 proto-topy-0.1.0/.coveragerc
+-rw-r--r--   0 decitre    (501) staff       (20)      636 2022-04-10 09:04:13.000000 proto-topy-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 decitre    (501) staff       (20)     1204 2022-04-12 06:44:18.000000 proto-topy-0.1.0/LICENSE
+-rw-r--r--   0 decitre    (501) staff       (20)      313 2022-11-17 16:44:09.000000 proto-topy-0.1.0/MANIFEST.in
+-rw-r--r--   0 decitre    (501) staff       (20)     2634 2023-06-08 16:27:47.959609 proto-topy-0.1.0/PKG-INFO
+-rw-r--r--   0 decitre    (501) staff       (20)     1710 2023-06-08 16:17:40.000000 proto-topy-0.1.0/README.md
+drwxr-xr-x   0 decitre    (501) staff       (20)        0 2023-06-08 16:27:47.951175 proto-topy-0.1.0/ci/
+-rwxr-xr-x   0 decitre    (501) staff       (20)     3063 2022-04-10 09:04:13.000000 proto-topy-0.1.0/ci/bootstrap.py
+-rw-r--r--   0 decitre    (501) staff       (20)       66 2022-04-10 09:04:13.000000 proto-topy-0.1.0/ci/requirements.txt
+drwxr-xr-x   0 decitre    (501) staff       (20)        0 2023-06-08 16:27:47.940703 proto-topy-0.1.0/ci/templates/
+drwxr-xr-x   0 decitre    (501) staff       (20)        0 2023-06-08 16:27:47.940908 proto-topy-0.1.0/ci/templates/.github/
+drwxr-xr-x   0 decitre    (501) staff       (20)        0 2023-06-08 16:27:47.952169 proto-topy-0.1.0/ci/templates/.github/workflows/
+-rw-r--r--   0 decitre    (501) staff       (20)     2001 2022-04-10 09:04:13.000000 proto-topy-0.1.0/ci/templates/.github/workflows/github-actions.yml
+-rw-r--r--   0 decitre    (501) staff       (20)      535 2023-06-08 16:22:26.000000 proto-topy-0.1.0/pyproject.toml
+-rw-r--r--   0 decitre    (501) staff       (20)        8 2022-04-10 17:23:50.000000 proto-topy-0.1.0/requirements.txt
+-rw-r--r--   0 decitre    (501) staff       (20)       15 2022-04-13 05:27:53.000000 proto-topy-0.1.0/requirements_test.txt
+-rw-r--r--   0 decitre    (501) staff       (20)      670 2023-06-08 16:27:47.960875 proto-topy-0.1.0/setup.cfg
+-rwxr-xr-x   0 decitre    (501) staff       (20)     3669 2023-06-08 16:17:40.000000 proto-topy-0.1.0/setup.py
+drwxr-xr-x   0 decitre    (501) staff       (20)        0 2023-06-08 16:27:47.941667 proto-topy-0.1.0/src/
+drwxr-xr-x   0 decitre    (501) staff       (20)        0 2023-06-08 16:27:47.953648 proto-topy-0.1.0/src/proto_topy/
+-rw-r--r--   0 decitre    (501) staff       (20)       22 2023-06-08 16:22:26.000000 proto-topy-0.1.0/src/proto_topy/__init__.py
+-rw-r--r--   0 decitre    (501) staff       (20)     9475 2023-06-08 16:17:40.000000 proto-topy-0.1.0/src/proto_topy/entities.py
+drwxr-xr-x   0 decitre    (501) staff       (20)        0 2023-06-08 16:27:47.957801 proto-topy-0.1.0/src/proto_topy.egg-info/
+-rw-r--r--   0 decitre    (501) staff       (20)     2634 2023-06-08 16:27:47.000000 proto-topy-0.1.0/src/proto_topy.egg-info/PKG-INFO
+-rw-r--r--   0 decitre    (501) staff       (20)      537 2023-06-08 16:27:47.000000 proto-topy-0.1.0/src/proto_topy.egg-info/SOURCES.txt
+-rw-r--r--   0 decitre    (501) staff       (20)        1 2023-06-08 16:27:47.000000 proto-topy-0.1.0/src/proto_topy.egg-info/dependency_links.txt
+-rw-r--r--   0 decitre    (501) staff       (20)        1 2023-06-08 16:27:47.000000 proto-topy-0.1.0/src/proto_topy.egg-info/not-zip-safe
+-rw-r--r--   0 decitre    (501) staff       (20)       38 2023-06-08 16:27:47.000000 proto-topy-0.1.0/src/proto_topy.egg-info/requires.txt
+-rw-r--r--   0 decitre    (501) staff       (20)       11 2023-06-08 16:27:47.000000 proto-topy-0.1.0/src/proto_topy.egg-info/top_level.txt
+drwxr-xr-x   0 decitre    (501) staff       (20)        0 2023-06-08 16:27:47.958528 proto-topy-0.1.0/tests/
+-rw-r--r--   0 decitre    (501) staff       (20)     8271 2023-06-08 16:17:40.000000 proto-topy-0.1.0/tests/test_proto_topy.py
+-rw-r--r--   0 decitre    (501) staff       (20)     1342 2023-06-08 16:17:40.000000 proto-topy-0.1.0/tox.ini
```

### Comparing `proto-topy-0.0.18/.pre-commit-config.yaml` & `proto-topy-0.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `proto-topy-0.0.18/LICENSE` & `proto-topy-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `proto-topy-0.0.18/PKG-INFO` & `proto-topy-0.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 Metadata-Version: 2.1
 Name: proto-topy
-Version: 0.0.18
+Version: 0.1.0
 Summary: Yet another tool that compiles .proto strings and import the outcome Python modules.
 Home-page: https://github.com/decitre/python-proto-topy
 Author: Emmanuel Decitre
 License: MIT
 Project-URL: Issue Tracker, https://github.com/decitre/python-proto-topy/issues
 Keywords: protobuf
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-Yet another tool that compiles .proto strings and import the outcome Python modules.
-
 [![test][test_badge]][test_target]
 [![version][version_badge]][pypi]
 [![wheel][wheel_badge]][pypi]
 [![python version][python_versions_badge]][pypi]
 [![python implementation][python_implementation_badge]][pypi]
 
+A tool that 
+- takes a `str` containing protobuf messages definitions 
+- returns a `types.ModuleType` instance
+
+It is useful for Python programs needing to parse protobuf messages without having to host `.proto` files in their code base.
+
 
 ## Installation
 
     pip install proto-topy
 
 ## Usage example
```

### Comparing `proto-topy-0.0.18/README.md` & `proto-topy-0.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,19 @@
-Yet another tool that compiles .proto strings and import the outcome Python modules.
-
 [![test][test_badge]][test_target]
 [![version][version_badge]][pypi]
 [![wheel][wheel_badge]][pypi]
 [![python version][python_versions_badge]][pypi]
 [![python implementation][python_implementation_badge]][pypi]
 
+A tool that 
+- takes a `str` containing protobuf messages definitions 
+- returns a `types.ModuleType` instance
+
+It is useful for Python programs needing to parse protobuf messages without having to host `.proto` files in their code base.
+
 
 ## Installation
 
     pip install proto-topy
 
 ## Usage example
```

### Comparing `proto-topy-0.0.18/ci/bootstrap.py` & `proto-topy-0.1.0/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `proto-topy-0.0.18/ci/templates/.github/workflows/github-actions.yml` & `proto-topy-0.1.0/ci/templates/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `proto-topy-0.0.18/setup.cfg` & `proto-topy-0.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `proto-topy-0.0.18/setup.py` & `proto-topy-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,22 +85,22 @@
         include_package_data=True,
         zip_safe=False,
         classifiers=[
             # complete classifier list: http://pypi.python.org/pypi?%3Aaction=list_classifiers
             'License :: OSI Approved :: MIT License',
             'Programming Language :: Python :: 3',
             "Programming Language :: Python :: 3 :: Only",
-            "Programming Language :: Python :: 3.7",
             "Programming Language :: Python :: 3.8",
             "Programming Language :: Python :: 3.9",
             "Programming Language :: Python :: 3.10",
+            "Programming Language :: Python :: 3.11",
             'Programming Language :: Python :: Implementation :: CPython',
             "Operating System :: OS Independent",
         ],
         project_urls={
             'Issue Tracker': f'{github_home}/python-{project_name}/issues',
         },
         keywords=['protobuf'],
-        python_requires='>=3.7',
+        python_requires='>=3.8',
         install_requires=requirements,
         extras_require={"dev": requirements_test},
     )
```

### Comparing `proto-topy-0.0.18/src/proto_topy/entities.py` & `proto-topy-0.1.0/src/proto_topy/entities.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,29 +128,43 @@
                 with open(
                     Path(dir, proto.package_path, f"{proto.name}_pb2.py")
                 ) as module_path:
                     proto.set_module(module_path.read(), global_scope=global_scope)
             sys.path.pop()
         return self
 
+
+    def version(self) -> str:
+        outs = ProtoCollection._do_compile(
+            self.compiler_path,
+            ["--version"],
+            [],
+            raise_exception=True,
+        )
+        if outs:
+            return outs.split()[-1].decode()
+
+
     @staticmethod
     def _do_compile(
         compiler_path: Path,
         compile_to_py_options: list,
         proto_source_files: list,
         raise_exception: bool = True,
-    ) -> None:
+    ) -> bytes:
+
         compile_command = [str(compiler_path.resolve())]
         compile_command.extend(compile_to_py_options)
         compile_command.extend(proto_source_files)
         compilation = Popen(compile_command, stdout=PIPE, stderr=PIPE)
         compilation.wait()
         outs, errs = compilation.communicate()
         if raise_exception:
             ProtoCollection._raise_for_errs(errs)
+        return outs
 
     @staticmethod
     def _raise_for_errs(errs: bytes) -> None:
         warnings = []
         errors = []
         if not errs:
             return
```

### Comparing `proto-topy-0.0.18/src/proto_topy.egg-info/PKG-INFO` & `proto-topy-0.1.0/src/proto_topy.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 Metadata-Version: 2.1
 Name: proto-topy
-Version: 0.0.18
+Version: 0.1.0
 Summary: Yet another tool that compiles .proto strings and import the outcome Python modules.
 Home-page: https://github.com/decitre/python-proto-topy
 Author: Emmanuel Decitre
 License: MIT
 Project-URL: Issue Tracker, https://github.com/decitre/python-proto-topy/issues
 Keywords: protobuf
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-Yet another tool that compiles .proto strings and import the outcome Python modules.
-
 [![test][test_badge]][test_target]
 [![version][version_badge]][pypi]
 [![wheel][wheel_badge]][pypi]
 [![python version][python_versions_badge]][pypi]
 [![python implementation][python_implementation_badge]][pypi]
 
+A tool that 
+- takes a `str` containing protobuf messages definitions 
+- returns a `types.ModuleType` instance
+
+It is useful for Python programs needing to parse protobuf messages without having to host `.proto` files in their code base.
+
 
 ## Installation
 
     pip install proto-topy
 
 ## Usage example
```

### Comparing `proto-topy-0.0.18/tox.ini` & `proto-topy-0.1.0/tox.ini`

 * *Files 14% similar despite different names*

```diff
@@ -9,24 +9,24 @@
     *
 ; a generative tox configuration, see: https://tox.readthedocs.io/en/latest/config.html#generative-envlist
 
 [tox]
 envlist =
     clean,
     check,
-    {py37,py38,py39,py310},
+    {3.8,3.9,3.10,3.11},
     report
 ignore_basepython_conflict = true
 
 [testenv]
 basepython =
-    py37: {env:TOXPYTHON:python3.7}
-    py38: {env:TOXPYTHON:python3.8}
-    py39: {env:TOXPYTHON:python3.9}
-    py310: {env:TOXPYTHON:python3.10}
+    3.8: {env:TOXPYTHON:python3.8}
+    3.9: {env:TOXPYTHON:python3.9}
+    3.10: {env:TOXPYTHON:python3.10}
+    3.11: {env:TOXPYTHON:python3.11}
     {bootstrap,clean,check,report,codecov}: {env:TOXPYTHON:python3}
 setenv =
     PYTHONPATH={toxinidir}/tests
     PYTHONUNBUFFERED=yes
 passenv =
     *
 usedevelop = false
```

