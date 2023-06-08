# Comparing `tmp/dagster-datahub-0.19.8.tar.gz` & `tmp/dagster-datahub-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-datahub-0.19.8.tar", last modified: Thu Jun  8 16:33:47 2023, max compression
+gzip compressed data, was "dagster-datahub-1.0.5.tar", last modified: Fri Aug 26 13:47:00 2022, max compression
```

## Comparing `dagster-datahub-0.19.8.tar` & `dagster-datahub-1.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:33:47.393926 dagster-datahub-0.19.8/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-06-08 16:23:49.000000 dagster-datahub-0.19.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)      214 2023-06-08 16:23:49.000000 dagster-datahub-0.19.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      703 2023-06-08 16:33:47.393926 dagster-datahub-0.19.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      131 2023-06-08 16:23:49.000000 dagster-datahub-0.19.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:33:47.393926 dagster-datahub-0.19.8/dagster_datahub/
--rw-r--r--   0 root         (0) root         (0)      492 2023-06-08 16:23:49.000000 dagster-datahub-0.19.8/dagster_datahub/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 16:23:49.000000 dagster-datahub-0.19.8/dagster_datahub/py.typed
--rw-r--r--   0 root         (0) root         (0)     3932 2023-06-08 16:23:49.000000 dagster-datahub-0.19.8/dagster_datahub/resources.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-08 16:23:49.000000 dagster-datahub-0.19.8/dagster_datahub/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:33:47.393926 dagster-datahub-0.19.8/dagster_datahub.egg-info/
--rw-r--r--   0 root         (0) root         (0)      703 2023-06-08 16:33:47.000000 dagster-datahub-0.19.8/dagster_datahub.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      389 2023-06-08 16:33:47.000000 dagster-datahub-0.19.8/dagster_datahub.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 16:33:47.000000 dagster-datahub-0.19.8/dagster_datahub.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 16:33:47.000000 dagster-datahub-0.19.8/dagster_datahub.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       84 2023-06-08 16:33:47.000000 dagster-datahub-0.19.8/dagster_datahub.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-08 16:33:47.000000 dagster-datahub-0.19.8/dagster_datahub.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      162 2023-06-08 16:33:47.393926 dagster-datahub-0.19.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1473 2023-06-08 16:23:49.000000 dagster-datahub-0.19.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:47:00.276965 dagster-datahub-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)    11357 2022-08-26 13:33:01.000000 dagster-datahub-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      214 2022-08-26 13:33:01.000000 dagster-datahub-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      679 2022-08-26 13:47:00.276965 dagster-datahub-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      131 2022-08-26 13:33:01.000000 dagster-datahub-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:47:00.276965 dagster-datahub-1.0.5/dagster_datahub/
+-rw-r--r--   0 root         (0) root         (0)      287 2022-08-26 13:33:01.000000 dagster-datahub-1.0.5/dagster_datahub/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-26 13:33:01.000000 dagster-datahub-1.0.5/dagster_datahub/py.typed
+-rw-r--r--   0 root         (0) root         (0)     3808 2022-08-26 13:33:01.000000 dagster-datahub-1.0.5/dagster_datahub/resources.py
+-rw-r--r--   0 root         (0) root         (0)       22 2022-08-26 13:33:01.000000 dagster-datahub-1.0.5/dagster_datahub/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:47:00.276965 dagster-datahub-1.0.5/dagster_datahub.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      679 2022-08-26 13:47:00.000000 dagster-datahub-1.0.5/dagster_datahub.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      389 2022-08-26 13:47:00.000000 dagster-datahub-1.0.5/dagster_datahub.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:47:00.000000 dagster-datahub-1.0.5/dagster_datahub.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:47:00.000000 dagster-datahub-1.0.5/dagster_datahub.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       85 2022-08-26 13:47:00.000000 dagster-datahub-1.0.5/dagster_datahub.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2022-08-26 13:47:00.000000 dagster-datahub-1.0.5/dagster_datahub.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      162 2022-08-26 13:47:00.276965 dagster-datahub-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1529 2022-08-26 13:33:01.000000 dagster-datahub-1.0.5/setup.py
```

### Comparing `dagster-datahub-0.19.8/LICENSE` & `dagster-datahub-1.0.5/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2023 Elementl, Inc.
+   Copyright {yyyy} {name of copyright owner}
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `dagster-datahub-0.19.8/PKG-INFO` & `dagster-datahub-1.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: dagster-datahub
-Version: 0.19.8
+Version: 1.0.5
 Summary: Package for Datahub-specific Dagster framework solid and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-datahub
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `dagster-datahub-0.19.8/dagster_datahub.egg-info/PKG-INFO` & `dagster-datahub-1.0.5/dagster_datahub.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: dagster-datahub
-Version: 0.19.8
+Version: 1.0.5
 Summary: Package for Datahub-specific Dagster framework solid and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-datahub
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
+
+UNKNOWN
+
```

