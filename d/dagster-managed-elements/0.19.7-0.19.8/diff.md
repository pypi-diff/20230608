# Comparing `tmp/dagster-managed-elements-0.19.7.tar.gz` & `tmp/dagster-managed-elements-0.19.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-managed-elements-0.19.7.tar", last modified: Thu Jun  1 18:26:42 2023, max compression
+gzip compressed data, was "dagster-managed-elements-0.19.8.tar", last modified: Thu Jun  8 16:32:25 2023, max compression
```

## Comparing `dagster-managed-elements-0.19.7.tar` & `dagster-managed-elements-0.19.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:26:42.365592 dagster-managed-elements-0.19.7/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-06-01 18:14:54.000000 dagster-managed-elements-0.19.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       76 2023-06-01 18:14:54.000000 dagster-managed-elements-0.19.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      686 2023-06-01 18:26:42.365592 dagster-managed-elements-0.19.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       27 2023-06-01 18:14:54.000000 dagster-managed-elements-0.19.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:26:42.365592 dagster-managed-elements-0.19.7/dagster_managed_elements/
--rw-r--r--   0 root         (0) root         (0)      202 2023-06-01 18:14:54.000000 dagster-managed-elements-0.19.7/dagster_managed_elements/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6327 2023-06-01 18:14:54.000000 dagster-managed-elements-0.19.7/dagster_managed_elements/cli.py
--rw-r--r--   0 root         (0) root         (0)     9573 2023-06-01 18:14:54.000000 dagster-managed-elements-0.19.7/dagster_managed_elements/types.py
--rw-r--r--   0 root         (0) root         (0)     3357 2023-06-01 18:14:54.000000 dagster-managed-elements-0.19.7/dagster_managed_elements/utils.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-01 18:14:54.000000 dagster-managed-elements-0.19.7/dagster_managed_elements/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:26:42.365592 dagster-managed-elements-0.19.7/dagster_managed_elements.egg-info/
--rw-r--r--   0 root         (0) root         (0)      686 2023-06-01 18:26:42.000000 dagster-managed-elements-0.19.7/dagster_managed_elements.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      558 2023-06-01 18:26:42.000000 dagster-managed-elements-0.19.7/dagster_managed_elements.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 18:26:42.000000 dagster-managed-elements-0.19.7/dagster_managed_elements.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      126 2023-06-01 18:26:42.000000 dagster-managed-elements-0.19.7/dagster_managed_elements.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 18:26:42.000000 dagster-managed-elements-0.19.7/dagster_managed_elements.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 18:26:42.000000 dagster-managed-elements-0.19.7/dagster_managed_elements.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-06-01 18:26:42.000000 dagster-managed-elements-0.19.7/dagster_managed_elements.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      171 2023-06-01 18:26:42.369592 dagster-managed-elements-0.19.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1518 2023-06-01 18:14:54.000000 dagster-managed-elements-0.19.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:32:25.577986 dagster-managed-elements-0.19.8/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-06-08 16:23:49.000000 dagster-managed-elements-0.19.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       76 2023-06-08 16:23:49.000000 dagster-managed-elements-0.19.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      686 2023-06-08 16:32:25.577986 dagster-managed-elements-0.19.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       27 2023-06-08 16:23:49.000000 dagster-managed-elements-0.19.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:32:25.573986 dagster-managed-elements-0.19.8/dagster_managed_elements/
+-rw-r--r--   0 root         (0) root         (0)      202 2023-06-08 16:23:49.000000 dagster-managed-elements-0.19.8/dagster_managed_elements/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6327 2023-06-08 16:23:49.000000 dagster-managed-elements-0.19.8/dagster_managed_elements/cli.py
+-rw-r--r--   0 root         (0) root         (0)     9573 2023-06-08 16:23:49.000000 dagster-managed-elements-0.19.8/dagster_managed_elements/types.py
+-rw-r--r--   0 root         (0) root         (0)     3357 2023-06-08 16:23:49.000000 dagster-managed-elements-0.19.8/dagster_managed_elements/utils.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-06-08 16:23:49.000000 dagster-managed-elements-0.19.8/dagster_managed_elements/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:32:25.577986 dagster-managed-elements-0.19.8/dagster_managed_elements.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      686 2023-06-08 16:32:25.000000 dagster-managed-elements-0.19.8/dagster_managed_elements.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      558 2023-06-08 16:32:25.000000 dagster-managed-elements-0.19.8/dagster_managed_elements.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 16:32:25.000000 dagster-managed-elements-0.19.8/dagster_managed_elements.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      126 2023-06-08 16:32:25.000000 dagster-managed-elements-0.19.8/dagster_managed_elements.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 16:32:25.000000 dagster-managed-elements-0.19.8/dagster_managed_elements.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 16:32:25.000000 dagster-managed-elements-0.19.8/dagster_managed_elements.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-06-08 16:32:25.000000 dagster-managed-elements-0.19.8/dagster_managed_elements.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      171 2023-06-08 16:32:25.577986 dagster-managed-elements-0.19.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1518 2023-06-08 16:23:49.000000 dagster-managed-elements-0.19.8/setup.py
```

### Comparing `dagster-managed-elements-0.19.7/LICENSE` & `dagster-managed-elements-0.19.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-managed-elements-0.19.7/PKG-INFO` & `dagster-managed-elements-0.19.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-managed-elements
-Version: 0.19.7
+Version: 0.19.8
 Summary: Package for Managed elements with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-managed-elements
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-managed-elements-0.19.7/dagster_managed_elements/cli.py` & `dagster-managed-elements-0.19.8/dagster_managed_elements/cli.py`

 * *Files identical despite different names*

### Comparing `dagster-managed-elements-0.19.7/dagster_managed_elements/types.py` & `dagster-managed-elements-0.19.8/dagster_managed_elements/types.py`

 * *Files identical despite different names*

### Comparing `dagster-managed-elements-0.19.7/dagster_managed_elements/utils.py` & `dagster-managed-elements-0.19.8/dagster_managed_elements/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-managed-elements-0.19.7/dagster_managed_elements.egg-info/PKG-INFO` & `dagster-managed-elements-0.19.8/dagster_managed_elements.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-managed-elements
-Version: 0.19.7
+Version: 0.19.8
 Summary: Package for Managed elements with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-managed-elements
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-managed-elements-0.19.7/dagster_managed_elements.egg-info/SOURCES.txt` & `dagster-managed-elements-0.19.8/dagster_managed_elements.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-managed-elements-0.19.7/setup.py` & `dagster-managed-elements-0.19.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_managed_elements_tests*"]),
-    install_requires=["dagster==1.3.7", "requests", "click_spinner"],
+    install_requires=["dagster==1.3.8", "requests", "click_spinner"],
     zip_safe=False,
     entry_points={
         "console_scripts": [
             "dagster-managed-elements = dagster_managed_elements.cli:main",
             "dagster-me = dagster_managed_elements.cli:main",
         ]
     },
```

