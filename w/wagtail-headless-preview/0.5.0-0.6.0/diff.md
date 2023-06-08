# Comparing `tmp/wagtail-headless-preview-0.5.0.tar.gz` & `tmp/wagtail-headless-preview-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-headless-preview-0.5.0.tar", last modified: Sun Nov 27 15:10:41 2022, max compression
+gzip compressed data, was "wagtail-headless-preview-0.6.0.tar", last modified: Thu Jun  8 11:53:44 2023, max compression
```

## Comparing `wagtail-headless-preview-0.5.0.tar` & `wagtail-headless-preview-0.6.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 15:10:41.290242 wagtail-headless-preview-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (122)      228 2022-11-27 15:10:38.000000 wagtail-headless-preview-0.5.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (122)     4294 2022-11-27 15:10:38.000000 wagtail-headless-preview-0.5.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     1545 2022-11-27 15:10:38.000000 wagtail-headless-preview-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      325 2022-11-27 15:10:38.000000 wagtail-headless-preview-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    14080 2022-11-27 15:10:41.290242 wagtail-headless-preview-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    10046 2022-11-27 15:10:38.000000 wagtail-headless-preview-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      493 2022-11-27 15:10:38.000000 wagtail-headless-preview-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      479 2022-11-27 15:10:41.290242 wagtail-headless-preview-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2027 2022-11-27 15:10:38.000000 wagtail-headless-preview-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 15:10:41.286242 wagtail-headless-preview-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 15:10:41.290242 wagtail-headless-preview-0.5.0/src/wagtail_headless_preview/
--rw-r--r--   0 runner    (1001) docker     (122)      240 2022-11-27 15:10:38.000000 wagtail-headless-preview-0.5.0/src/wagtail_headless_preview/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 15:10:41.290242 wagtail-headless-preview-0.5.0/src/wagtail_headless_preview/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (122)      520 2022-11-27 15:10:41.000000 wagtail-headless-preview-0.5.0/src/wagtail_headless_preview/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      665 2022-11-27 15:10:41.000000 wagtail-headless-preview-0.5.0/src/wagtail_headless_preview/__pycache__/deprecation.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      175 2022-11-27 15:10:38.000000 wagtail-headless-preview-0.5.0/src/wagtail_headless_preview/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)      315 2022-11-27 15:10:38.000000 wagtail-headless-preview-0.5.0/src/wagtail_headless_preview/deprecation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 15:10:41.290242 wagtail-headless-preview-0.5.0/src/wagtail_headless_preview/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     1141 2022-11-27 15:10:38.000000 wagtail-headless-preview-0.5.0/src/wagtail_headless_preview/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-27 15:10:38.000000 wagtail-headless-preview-0.5.0/src/wagtail_headless_preview/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4848 2022-11-27 15:10:38.000000 wagtail-headless-preview-0.5.0/src/wagtail_headless_preview/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     4163 2022-11-27 15:10:38.000000 wagtail-headless-preview-0.5.0/src/wagtail_headless_preview/settings.py
--rw-r--r--   0 runner    (1001) docker     (122)       63 2022-11-27 15:10:38.000000 wagtail-headless-preview-0.5.0/src/wagtail_headless_preview/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 15:10:41.286242 wagtail-headless-preview-0.5.0/src/wagtail_headless_preview/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 15:10:41.290242 wagtail-headless-preview-0.5.0/src/wagtail_headless_preview/templates/wagtail_headless_preview/
--rw-r--r--   0 runner    (1001) docker     (122)      194 2022-11-27 15:10:38.000000 wagtail-headless-preview-0.5.0/src/wagtail_headless_preview/templates/wagtail_headless_preview/preview.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 15:10:41.290242 wagtail-headless-preview-0.5.0/src/wagtail_headless_preview.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    14080 2022-11-27 15:10:41.000000 wagtail-headless-preview-0.5.0/src/wagtail_headless_preview.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      909 2022-11-27 15:10:41.000000 wagtail-headless-preview-0.5.0/src/wagtail_headless_preview.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-27 15:10:41.000000 wagtail-headless-preview-0.5.0/src/wagtail_headless_preview.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       49 2022-11-27 15:10:41.000000 wagtail-headless-preview-0.5.0/src/wagtail_headless_preview.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       25 2022-11-27 15:10:41.000000 wagtail-headless-preview-0.5.0/src/wagtail_headless_preview.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:53:44.190081 wagtail-headless-preview-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-08 11:53:36.000000 wagtail-headless-preview-0.6.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-06-08 11:53:36.000000 wagtail-headless-preview-0.6.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-08 11:53:36.000000 wagtail-headless-preview-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-08 11:53:36.000000 wagtail-headless-preview-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14020 2023-06-08 11:53:44.190081 wagtail-headless-preview-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-06-08 11:53:36.000000 wagtail-headless-preview-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-08 11:53:36.000000 wagtail-headless-preview-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-08 11:53:44.190081 wagtail-headless-preview-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-08 11:53:36.000000 wagtail-headless-preview-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:53:44.186081 wagtail-headless-preview-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:53:44.190081 wagtail-headless-preview-0.6.0/src/wagtail_headless_preview/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-08 11:53:36.000000 wagtail-headless-preview-0.6.0/src/wagtail_headless_preview/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:53:44.190081 wagtail-headless-preview-0.6.0/src/wagtail_headless_preview/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-08 11:53:43.000000 wagtail-headless-preview-0.6.0/src/wagtail_headless_preview/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-08 11:53:43.000000 wagtail-headless-preview-0.6.0/src/wagtail_headless_preview/__pycache__/deprecation.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-08 11:53:36.000000 wagtail-headless-preview-0.6.0/src/wagtail_headless_preview/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-08 11:53:36.000000 wagtail-headless-preview-0.6.0/src/wagtail_headless_preview/deprecation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:53:44.190081 wagtail-headless-preview-0.6.0/src/wagtail_headless_preview/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-08 11:53:36.000000 wagtail-headless-preview-0.6.0/src/wagtail_headless_preview/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 11:53:36.000000 wagtail-headless-preview-0.6.0/src/wagtail_headless_preview/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-06-08 11:53:36.000000 wagtail-headless-preview-0.6.0/src/wagtail_headless_preview/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-06-08 11:53:36.000000 wagtail-headless-preview-0.6.0/src/wagtail_headless_preview/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-08 11:53:36.000000 wagtail-headless-preview-0.6.0/src/wagtail_headless_preview/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:53:44.186081 wagtail-headless-preview-0.6.0/src/wagtail_headless_preview/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:53:44.190081 wagtail-headless-preview-0.6.0/src/wagtail_headless_preview/templates/wagtail_headless_preview/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-08 11:53:36.000000 wagtail-headless-preview-0.6.0/src/wagtail_headless_preview/templates/wagtail_headless_preview/preview.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:53:44.190081 wagtail-headless-preview-0.6.0/src/wagtail_headless_preview.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14020 2023-06-08 11:53:43.000000 wagtail-headless-preview-0.6.0/src/wagtail_headless_preview.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-08 11:53:44.000000 wagtail-headless-preview-0.6.0/src/wagtail_headless_preview.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 11:53:43.000000 wagtail-headless-preview-0.6.0/src/wagtail_headless_preview.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-08 11:53:43.000000 wagtail-headless-preview-0.6.0/src/wagtail_headless_preview.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-08 11:53:43.000000 wagtail-headless-preview-0.6.0/src/wagtail_headless_preview.egg-info/top_level.txt
```

### Comparing `wagtail-headless-preview-0.5.0/CHANGELOG.md` & `wagtail-headless-preview-0.6.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.6] - 2023-06-08
+
+- Add Wagtail 4.2 support and drop support for Wagtail < 4.1
+- The minimum supported Python version is 3.8
+- Switched to using ruff
+
 ## [0.5] - 2022-11-27
 
 ### Fixed
 
 - Race condition in `create_page_view` ([#35](https://github.com/torchbox/wagtail-headless-preview/pull/35)) @johncarter-phntm
 
 ### Removed
```

### Comparing `wagtail-headless-preview-0.5.0/LICENSE` & `wagtail-headless-preview-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-headless-preview-0.5.0/PKG-INFO` & `wagtail-headless-preview-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: wagtail-headless-preview
-Version: 0.5.0
+Version: 0.6.0
 Summary: Enhance Wagtail previews in headless setups.
 Home-page: https://github.com/torchbox/wagtail-headless-preview
 Author: Dan Braghis
 Author-email: dan.braghis@torchbox.com
 License: BSD
 Project-URL: Changelog, https://github.com/torchbox/wagtail-headless-preview/blob/main/CHANGELOG.md
 Description: # [Wagtail Headless Preview](https://pypi.org/project/wagtail-headless-preview/)
         
-        [![Build status](https://img.shields.io/github/workflow/status/torchbox/wagtail-headless-preview/CI/main?style=for-the-badge)](https://github.com/torchbox/wagtail-headless-preview/actions)
+        [![Build status](https://img.shields.io/github/actions/workflow/status/torchbox/wagtail-headless-preview/ci.yml?style=for-the-badge)](https://github.com/torchbox/wagtail-headless-preview/actions)
         [![PyPI](https://img.shields.io/pypi/v/wagtail-headless-preview.svg?style=for-the-badge)](https://pypi.org/project/wagtail-headless-preview/)
         [![black](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge)](https://github.com/psf/black)
         [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/torchbox/wagtail-headless-preview/main.svg)](https://results.pre-commit.ci/latest/github/torchbox/wagtail-headless-preview/main)
         
         
         ## Overview
         
@@ -318,16 +318,16 @@
         
         Now you can run tests as shown below:
         
         ```sh
         tox -p
         ```
         
-        or, you can run them for a specific environment `tox -e py39-django3.2-wagtail2.15` or specific test
-        `tox -e py310-django3.2-wagtail2.15 wagtail_headless_preview.tests.test_frontend.TestFrontendViews.test_redirect_on_preview`
+        or, you can run them for a specific environment `tox -e py39-django3.2-wagtail4.1` or specific test
+        `tox -e py310-django3.2-wagtail4.1 wagtail_headless_preview.tests.test_frontend.TestFrontendViews.test_redirect_on_preview`
         
         ## Credits
         
         - Matthew Westcott ([@gasman](https://github.com/gasman)), initial proof of concept
         - Karl Hobley ([@kaedroho](https://github.com/kaedroho)), PoC improvements
         
 Keywords: wagtail,django,headless
@@ -335,24 +335,23 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Wagtail
-Classifier: Framework :: Wagtail :: 2
-Classifier: Framework :: Wagtail :: 3
 Classifier: Framework :: Wagtail :: 4
+Classifier: Framework :: Wagtail :: 5
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: testing
```

### Comparing `wagtail-headless-preview-0.5.0/README.md` & `wagtail-headless-preview-0.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # [Wagtail Headless Preview](https://pypi.org/project/wagtail-headless-preview/)
 
-[![Build status](https://img.shields.io/github/workflow/status/torchbox/wagtail-headless-preview/CI/main?style=for-the-badge)](https://github.com/torchbox/wagtail-headless-preview/actions)
+[![Build status](https://img.shields.io/github/actions/workflow/status/torchbox/wagtail-headless-preview/ci.yml?style=for-the-badge)](https://github.com/torchbox/wagtail-headless-preview/actions)
 [![PyPI](https://img.shields.io/pypi/v/wagtail-headless-preview.svg?style=for-the-badge)](https://pypi.org/project/wagtail-headless-preview/)
 [![black](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge)](https://github.com/psf/black)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/torchbox/wagtail-headless-preview/main.svg)](https://results.pre-commit.ci/latest/github/torchbox/wagtail-headless-preview/main)
 
 
 ## Overview
 
@@ -309,14 +309,14 @@
 
 Now you can run tests as shown below:
 
 ```sh
 tox -p
 ```
 
-or, you can run them for a specific environment `tox -e py39-django3.2-wagtail2.15` or specific test
-`tox -e py310-django3.2-wagtail2.15 wagtail_headless_preview.tests.test_frontend.TestFrontendViews.test_redirect_on_preview`
+or, you can run them for a specific environment `tox -e py39-django3.2-wagtail4.1` or specific test
+`tox -e py310-django3.2-wagtail4.1 wagtail_headless_preview.tests.test_frontend.TestFrontendViews.test_redirect_on_preview`
 
 ## Credits
 
 - Matthew Westcott ([@gasman](https://github.com/gasman)), initial proof of concept
 - Karl Hobley ([@kaedroho](https://github.com/kaedroho)), PoC improvements
```

### Comparing `wagtail-headless-preview-0.5.0/setup.py` & `wagtail-headless-preview-0.6.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,41 +16,40 @@
     description="Enhance Wagtail previews in headless setups.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Dan Braghis",
     author_email="dan.braghis@torchbox.com",
     url="https://github.com/torchbox/wagtail-headless-preview",
     project_urls={
-        "Changelog": "https://github.com/torchbox/wagtail-headless-preview/blob/main/CHANGELOG.md",  # noqa:B950
+        "Changelog": "https://github.com/torchbox/wagtail-headless-preview/blob/main/CHANGELOG.md",  # noqa:B950 E501
     },
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     include_package_data=True,
     license="BSD",
-    install_requires=["wagtail>=2.15"],
+    python_requires=">=3.8",
+    install_requires=["wagtail>=4.1"],
     extras_require={"testing": ["tox", "django-cors-headers"]},
     keywords=["wagtail", "django", "headless"],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Framework :: Django",
         "Framework :: Django :: 3.2",
-        "Framework :: Django :: 4.0",
         "Framework :: Django :: 4.1",
+        "Framework :: Django :: 4.2",
         "Framework :: Wagtail",
-        "Framework :: Wagtail :: 2",
-        "Framework :: Wagtail :: 3",
         "Framework :: Wagtail :: 4",
+        "Framework :: Wagtail :: 5",
         "Topic :: Internet :: WWW/HTTP",
         "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
     ],
 )
```

### Comparing `wagtail-headless-preview-0.5.0/src/wagtail_headless_preview/__pycache__/__init__.cpython-38.pyc` & `wagtail-headless-preview-0.6.0/src/wagtail_headless_preview/__pycache__/__init__.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Sun Nov 27 15:10:38 2022 UTC, .py size: 240 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-00000000: 550d 0d0a 0000 0000 ee7d 8363 f000 0000  U........}.c....
+00000000: 550d 0d0a 0000 0000 40c1 8164 f000 0000  U.......@..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 5a00 6401 a001 6502 6503 6500 8302 a101  Z.d...e.e.e.....
 00000040: 5a04 6402 6403 8400 5a05 6505 8300 0100  Z.d.d...Z.e.....
-00000050: 6404 5300 2905 2903 e900 0000 00e9 0500  d.S.).).........
+00000050: 6404 5300 2905 2903 e900 0000 00e9 0600  d.S.).).........
 00000060: 0000 7201 0000 00da 012e 6300 0000 0000  ..r.......c.....
 00000070: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
 00000080: 0000 0073 2400 0000 6401 6400 6c00 7d00  ...s$...d.d.l.}.
 00000090: 6402 6403 6c01 6d02 7d01 0100 7c00 a003  d.d.l.m.}...|...
 000000a0: 6404 7c01 a102 0100 6400 5300 2905 4e72  d.|.....d.S.).Nr
 000000b0: 0100 0000 e901 0000 0029 01da 1f72 656d  .........)...rem
 000000c0: 6f76 6564 5f69 6e5f 6e65 7874 5f76 6572  oved_in_next_ver
```

### Comparing `wagtail-headless-preview-0.5.0/src/wagtail_headless_preview/__pycache__/deprecation.cpython-38.pyc` & `wagtail-headless-preview-0.6.0/src/wagtail_headless_preview/__pycache__/deprecation.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Sun Nov 27 15:10:38 2022 UTC, .py size: 315 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-00000000: 550d 0d0a 0000 0000 ee7d 8363 3b01 0000  U........}.c;...
+00000000: 550d 0d0a 0000 0000 40c1 8164 3b01 0000  U.......@..d;...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2c00 0000 4700  .....@...s,...G.
 00000030: 6400 6401 8400 6401 6500 8303 5a01 4700  d.d...d.e...Z.G.
 00000040: 6402 6403 8400 6403 6502 8303 5a03 6501  d.d...d.e...Z.e.
 00000050: 5a04 6503 5a05 6404 5300 2905 6300 0000  Z.e.Z.d.S.).c...
 00000060: 0000 0000 0000 0000 0000 0000 0001 0000  ................
 00000070: 0040 0000 0073 0c00 0000 6500 5a01 6400  .@...s....e.Z.d.
 00000080: 5a02 6401 5300 2902 da29 5265 6d6f 7665  Z.d.S.)..)Remove
 00000090: 6449 6e57 6167 7461 696c 4865 6164 6c65  dInWagtailHeadle
-000000a0: 7373 5072 6576 6965 7730 3630 5761 726e  ssPreview060Warn
+000000a0: 7373 5072 6576 6965 7730 3730 5761 726e  ssPreview070Warn
 000000b0: 696e 674e a903 da08 5f5f 6e61 6d65 5f5f  ingN....__name__
 000000c0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
 000000d0: 7175 616c 6e61 6d65 5f5f a900 7206 0000  qualname__..r...
 000000e0: 0072 0600 0000 fa6f 2f68 6f6d 652f 7275  .r.....o/home/ru
 000000f0: 6e6e 6572 2f77 6f72 6b2f 7761 6774 6169  nner/work/wagtai
 00000100: 6c2d 6865 6164 6c65 7373 2d70 7265 7669  l-headless-previ
 00000110: 6577 2f77 6167 7461 696c 2d68 6561 646c  ew/wagtail-headl
@@ -21,15 +21,15 @@
 00000140: 5f70 7265 7669 6577 2f64 6570 7265 6361  _preview/depreca
 00000150: 7469 6f6e 2e70 7972 0100 0000 0100 0000  tion.pyr........
 00000160: 7302 0000 0008 0172 0100 0000 6300 0000  s......r....c...
 00000170: 0000 0000 0000 0000 0000 0000 0001 0000  ................
 00000180: 0040 0000 0073 0c00 0000 6500 5a01 6400  .@...s....e.Z.d.
 00000190: 5a02 6401 5300 2902 da29 5265 6d6f 7665  Z.d.S.)..)Remove
 000001a0: 6449 6e57 6167 7461 696c 4865 6164 6c65  dInWagtailHeadle
-000001b0: 7373 5072 6576 6965 7730 3730 5761 726e  ssPreview070Warn
+000001b0: 7373 5072 6576 6965 7730 3830 5761 726e  ssPreview080Warn
 000001c0: 696e 674e 7202 0000 0072 0600 0000 7206  ingNr....r....r.
 000001d0: 0000 0072 0600 0000 7207 0000 0072 0800  ...r....r....r..
 000001e0: 0000 0500 0000 7302 0000 0008 0172 0800  ......s......r..
 000001f0: 0000 4e29 06da 1244 6570 7265 6361 7469  ..N)...Deprecati
 00000200: 6f6e 5761 726e 696e 6772 0100 0000 da19  onWarningr......
 00000210: 5065 6e64 696e 6744 6570 7265 6361 7469  PendingDeprecati
 00000220: 6f6e 5761 726e 696e 6772 0800 0000 da1f  onWarningr......
```

### Comparing `wagtail-headless-preview-0.5.0/src/wagtail_headless_preview/migrations/0001_initial.py` & `wagtail-headless-preview-0.6.0/src/wagtail_headless_preview/migrations/0001_initial.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Generated by Django 2.1.5 on 2019-03-19 14:21
 
-from django.db import migrations, models
 import django.db.models.deletion
 
+from django.db import migrations, models
+
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = [("contenttypes", "0002_remove_content_type_name")]
 
     operations = [
         migrations.CreateModel(
             name="PagePreview",
```

### Comparing `wagtail-headless-preview-0.5.0/src/wagtail_headless_preview/models.py` & `wagtail-headless-preview-0.6.0/src/wagtail_headless_preview/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,16 +76,16 @@
             identifier = (
                 f"parent_id={self.get_parent().pk};page_type={self._meta.label}"
             )
         else:
             identifier = f"id={self.pk}"
 
         token = self.get_preview_signer().sign(identifier)
-        # Note: Using update_page_preview() instead of just create() to avoid unique constraint
-        # failures if preview is clicked multiple times
+        # Note: Using update_page_preview() instead of just create() to avoid
+        # unique constraint failures if preview is clicked multiple times
         preview, _ = self.update_page_preview(token)
 
         return preview
 
     def update_page_preview(self, token):
         return PagePreview.objects.update_or_create(
             token=token,
@@ -128,16 +128,17 @@
 
 class HeadlessServeMixin:
     def serve(self, request):
         """
         Mixin overriding the default serve method with a redirect.
         The URL of the requested page is kept the same, only the host is
         overridden.
-        By default this uses the hosts defined in HEADLESS_PREVIEW_CLIENT_URLS.
-        However, you can enforce a single host using  the HEADLESS_SERVE_BASE_URL setting.
+        By default, this uses the hosts defined in HEADLESS_PREVIEW_CLIENT_URLS.
+        However, you can enforce a single host using the HEADLESS_SERVE_BASE_URL
+        setting.
         """
         if headless_preview_settings.SERVE_BASE_URL:
             base_url = headless_preview_settings.SERVE_BASE_URL
         else:
             base_url = get_client_root_url_from_site(self.get_site())
         site_id, site_root, relative_page_url = self.get_url_parts(request)
         return redirect(f"{base_url.rstrip('/')}{relative_page_url}")
```

### Comparing `wagtail-headless-preview-0.5.0/src/wagtail_headless_preview/settings.py` & `wagtail-headless-preview-0.6.0/src/wagtail_headless_preview/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """
-The wagtail_headless_preview settings are namespaced in the WAGTAIL_HEADLESS_PREVIEW setting.
+The wagtail_headless_preview settings are namespaced in the
+WAGTAIL_HEADLESS_PREVIEW setting.
+
 For example your project's `settings.py` file might look like this:
 WAGTAIL_HEADLESS_PREVIEW = {
     "CLIENT_URLS": {"default": "https://headless.site"},
     # ...
 }
 This module provides the `headless_preview_settings` object, that is used to access
 the settings. It checks for user settings first, with fallback to defaults.
@@ -26,16 +28,16 @@
 
 # List of settings that have been removed
 REMOVED_SETTINGS = ["HEADLESS_PREVIEW_CLIENT_URLS"]
 
 
 class WagtailHeadlessPreviewSettings:
     """
-    A settings object that allows the wagtail_headless_preview settings to be accessed as
-    properties. For example:
+    A settings object that allows the wagtail_headless_preview settings to be
+    accessed as properties. For example:
         from wagtail_headless_previews.settings import headless_preview_settings
         print(headless_preview_settings.CLIENT_URLS)
     Note:
     This is an internal class that is only compatible with settings namespaced
     under the WAGTAIL_HEADLESS_PREVIEW name. It is not intended to be used by 3rd-party
     apps, and test helpers like `override_settings` may not work as expected.
     """
@@ -77,14 +79,15 @@
             setting_in_user_settings = old_setting in user_settings
             if setting_in_user_settings or hasattr(settings, old_setting):
                 warnings.warn(
                     f"The '{old_setting}' setting is deprecated and will be "
                     f"removed in the next release, use "
                     f'WAGTAIL_HEADLESS_PREVIEW["{new_setting}"] instead.',
                     category=category,
+                    stacklevel=2,
                 )
                 if setting_in_user_settings:
                     user_settings[new_setting] = user_settings[old_setting]
                 else:
                     user_settings[new_setting] = getattr(settings, old_setting)
 
         for removed_setting in REMOVED_SETTINGS:
```

### Comparing `wagtail-headless-preview-0.5.0/src/wagtail_headless_preview.egg-info/PKG-INFO` & `wagtail-headless-preview-0.6.0/src/wagtail_headless_preview.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: wagtail-headless-preview
-Version: 0.5.0
+Version: 0.6.0
 Summary: Enhance Wagtail previews in headless setups.
 Home-page: https://github.com/torchbox/wagtail-headless-preview
 Author: Dan Braghis
 Author-email: dan.braghis@torchbox.com
 License: BSD
 Project-URL: Changelog, https://github.com/torchbox/wagtail-headless-preview/blob/main/CHANGELOG.md
 Description: # [Wagtail Headless Preview](https://pypi.org/project/wagtail-headless-preview/)
         
-        [![Build status](https://img.shields.io/github/workflow/status/torchbox/wagtail-headless-preview/CI/main?style=for-the-badge)](https://github.com/torchbox/wagtail-headless-preview/actions)
+        [![Build status](https://img.shields.io/github/actions/workflow/status/torchbox/wagtail-headless-preview/ci.yml?style=for-the-badge)](https://github.com/torchbox/wagtail-headless-preview/actions)
         [![PyPI](https://img.shields.io/pypi/v/wagtail-headless-preview.svg?style=for-the-badge)](https://pypi.org/project/wagtail-headless-preview/)
         [![black](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge)](https://github.com/psf/black)
         [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/torchbox/wagtail-headless-preview/main.svg)](https://results.pre-commit.ci/latest/github/torchbox/wagtail-headless-preview/main)
         
         
         ## Overview
         
@@ -318,16 +318,16 @@
         
         Now you can run tests as shown below:
         
         ```sh
         tox -p
         ```
         
-        or, you can run them for a specific environment `tox -e py39-django3.2-wagtail2.15` or specific test
-        `tox -e py310-django3.2-wagtail2.15 wagtail_headless_preview.tests.test_frontend.TestFrontendViews.test_redirect_on_preview`
+        or, you can run them for a specific environment `tox -e py39-django3.2-wagtail4.1` or specific test
+        `tox -e py310-django3.2-wagtail4.1 wagtail_headless_preview.tests.test_frontend.TestFrontendViews.test_redirect_on_preview`
         
         ## Credits
         
         - Matthew Westcott ([@gasman](https://github.com/gasman)), initial proof of concept
         - Karl Hobley ([@kaedroho](https://github.com/kaedroho)), PoC improvements
         
 Keywords: wagtail,django,headless
@@ -335,24 +335,23 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Wagtail
-Classifier: Framework :: Wagtail :: 2
-Classifier: Framework :: Wagtail :: 3
 Classifier: Framework :: Wagtail :: 4
+Classifier: Framework :: Wagtail :: 5
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: testing
```

### Comparing `wagtail-headless-preview-0.5.0/src/wagtail_headless_preview.egg-info/SOURCES.txt` & `wagtail-headless-preview-0.6.0/src/wagtail_headless_preview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

