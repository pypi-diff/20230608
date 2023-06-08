# Comparing `tmp/dagster-datahub-0.19.9rc0.tar.gz` & `tmp/dagster-datahub-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-datahub-0.19.9rc0.tar", last modified: Thu Jun  8 18:30:25 2023, max compression
+gzip compressed data, was "dagster-datahub-1.0.5.tar", last modified: Fri Aug 26 13:47:00 2022, max compression
```

## Comparing `dagster-datahub-0.19.9rc0.tar` & `dagster-datahub-1.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:30:25.800431 dagster-datahub-0.19.9rc0/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-06-08 18:20:46.000000 dagster-datahub-0.19.9rc0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      214 2023-06-08 18:20:46.000000 dagster-datahub-0.19.9rc0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      706 2023-06-08 18:30:25.800431 dagster-datahub-0.19.9rc0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      131 2023-06-08 18:20:46.000000 dagster-datahub-0.19.9rc0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:30:25.800431 dagster-datahub-0.19.9rc0/dagster_datahub/
--rw-r--r--   0 root         (0) root         (0)      492 2023-06-08 18:20:46.000000 dagster-datahub-0.19.9rc0/dagster_datahub/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:20:46.000000 dagster-datahub-0.19.9rc0/dagster_datahub/py.typed
--rw-r--r--   0 root         (0) root         (0)     3932 2023-06-08 18:20:46.000000 dagster-datahub-0.19.9rc0/dagster_datahub/resources.py
--rw-r--r--   0 root         (0) root         (0)       26 2023-06-08 18:20:46.000000 dagster-datahub-0.19.9rc0/dagster_datahub/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:30:25.800431 dagster-datahub-0.19.9rc0/dagster_datahub.egg-info/
--rw-r--r--   0 root         (0) root         (0)      706 2023-06-08 18:30:25.000000 dagster-datahub-0.19.9rc0/dagster_datahub.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      389 2023-06-08 18:30:25.000000 dagster-datahub-0.19.9rc0/dagster_datahub.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:30:25.000000 dagster-datahub-0.19.9rc0/dagster_datahub.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:30:25.000000 dagster-datahub-0.19.9rc0/dagster_datahub.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       87 2023-06-08 18:30:25.000000 dagster-datahub-0.19.9rc0/dagster_datahub.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-08 18:30:25.000000 dagster-datahub-0.19.9rc0/dagster_datahub.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      162 2023-06-08 18:30:25.800431 dagster-datahub-0.19.9rc0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1476 2023-06-08 18:20:46.000000 dagster-datahub-0.19.9rc0/setup.py
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

### Comparing `dagster-datahub-0.19.9rc0/LICENSE` & `dagster-datahub-1.0.5/LICENSE`

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

### Comparing `dagster-datahub-0.19.9rc0/PKG-INFO` & `dagster-datahub-1.0.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: dagster-datahub
-Version: 0.19.9rc0
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

### Comparing `dagster-datahub-0.19.9rc0/dagster_datahub.egg-info/PKG-INFO` & `dagster-datahub-1.0.5/dagster_datahub.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: dagster-datahub
-Version: 0.19.9rc0
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

### Comparing `dagster-datahub-0.19.9rc0/setup.py` & `dagster-datahub-1.0.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,44 @@
-from pathlib import Path
 from typing import Dict
 
 from setuptools import find_packages, setup
 
 
 def get_version() -> str:
     version: Dict[str, str] = {}
-    with open(Path(__file__).parent / "dagster_datahub/version.py", encoding="utf8") as fp:
-        exec(fp.read(), version)
+    with open("dagster_datahub/version.py", encoding="utf8") as fp:
+        exec(fp.read(), version)  # pylint: disable=W0122
 
     return version["__version__"]
 
 
-ver = get_version()
-# dont pin dev installs to avoid pip dep resolver issues
-pin = "" if ver == "1!0+dev" else f"=={ver}"
-setup(
-    name="dagster-datahub",
-    version=ver,
-    author="Elementl",
-    author_email="hello@elementl.com",
-    license="Apache-2.0",
-    description="Package for Datahub-specific Dagster framework solid and resource components.",
-    url=(
-        "https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-datahub"
-    ),
-    classifiers=[
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-        "License :: OSI Approved :: Apache Software License",
-        "Operating System :: OS Independent",
-    ],
-    packages=find_packages(exclude=["dagster_datahub_tests*"]),
-    include_package_data=True,
-    install_requires=[
-        "acryl-datahub[datahub-rest, datahub-kafka]<=0.10.2",
-        "dagster==1.3.9rc0",
-        "packaging",
-        "requests",
-    ],
-    extras_require={},
-    zip_safe=False,
-)
+if __name__ == "__main__":
+    ver = get_version()
+    # dont pin dev installs to avoid pip dep resolver issues
+    pin = "" if ver == "0+dev" else f"=={ver}"
+    setup(
+        name="dagster-datahub",
+        version=ver,
+        author="Elementl",
+        author_email="hello@elementl.com",
+        license="Apache-2.0",
+        description="Package for Datahub-specific Dagster framework solid and resource components.",
+        url="https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-datahub",
+        classifiers=[
+            "Programming Language :: Python :: 3.7",
+            "Programming Language :: Python :: 3.8",
+            "Programming Language :: Python :: 3.9",
+            "Programming Language :: Python :: 3.10",
+            "License :: OSI Approved :: Apache Software License",
+            "Operating System :: OS Independent",
+        ],
+        packages=find_packages(exclude=["dagster_datahub_tests*"]),
+        include_package_data=True,
+        install_requires=[
+            "acryl-datahub[datahub-rest, datahub-kafka]<0.8.41.2",
+            "dagster==1.0.5",
+            "packaging",
+            "requests",
+        ],
+        extras_require={},
+        zip_safe=False,
+    )
```

