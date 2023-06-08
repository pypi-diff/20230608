# Comparing `tmp/ape-polygon-0.6.1.tar.gz` & `tmp/ape-polygon-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-polygon-0.6.1.tar", last modified: Wed Apr 12 21:30:16 2023, max compression
+gzip compressed data, was "ape-polygon-0.6.2.tar", last modified: Thu Jun  8 19:29:29 2023, max compression
```

## Comparing `ape-polygon-0.6.1.tar` & `ape-polygon-0.6.2.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:30:16.860195 ape-polygon-0.6.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:30:16.860195 ape-polygon-0.6.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:30:16.860195 ape-polygon-0.6.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:30:16.860195 ape-polygon-0.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-12 21:30:16.860195 ape-polygon-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:30:16.860195 ape-polygon-0.6.1/ape_polygon/
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/ape_polygon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/ape_polygon/ecosystem.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/ape_polygon/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-12 21:30:16.000000 ape-polygon-0.6.1/ape_polygon/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:30:16.860195 ape-polygon-0.6.1/ape_polygon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-12 21:30:16.000000 ape-polygon-0.6.1/ape_polygon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-12 21:30:16.000000 ape-polygon-0.6.1/ape_polygon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 21:30:16.000000 ape-polygon-0.6.1/ape_polygon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 21:30:16.000000 ape-polygon-0.6.1/ape_polygon.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-12 21:30:16.000000 ape-polygon-0.6.1/ape_polygon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-12 21:30:16.000000 ape-polygon-0.6.1/ape_polygon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-12 21:30:16.860195 ape-polygon-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:30:16.860195 ape-polygon-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/tests/test_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:29:29.127385 ape-polygon-0.6.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:29:29.123385 ape-polygon-0.6.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:29:29.123385 ape-polygon-0.6.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:29:29.127385 ape-polygon-0.6.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-06-08 19:29:29.127385 ape-polygon-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:29:29.127385 ape-polygon-0.6.2/ape_polygon/
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/ape_polygon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/ape_polygon/ecosystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/ape_polygon/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-08 19:29:28.000000 ape-polygon-0.6.2/ape_polygon/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:29:29.127385 ape-polygon-0.6.2/ape_polygon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-06-08 19:29:29.000000 ape-polygon-0.6.2/ape_polygon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-08 19:29:29.000000 ape-polygon-0.6.2/ape_polygon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 19:29:29.000000 ape-polygon-0.6.2/ape_polygon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 19:29:29.000000 ape-polygon-0.6.2/ape_polygon.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-08 19:29:29.000000 ape-polygon-0.6.2/ape_polygon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-08 19:29:29.000000 ape-polygon-0.6.2/ape_polygon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-08 19:29:29.131385 ape-polygon-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:29:29.127385 ape-polygon-0.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/tests/test_ecosystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/tests/test_provider.py
```

### Comparing `ape-polygon-0.6.1/.github/ISSUE_TEMPLATE/bug.md` & `ape-polygon-0.6.2/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.1/.github/ISSUE_TEMPLATE/feature.md` & `ape-polygon-0.6.2/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.1/.github/ISSUE_TEMPLATE/work-item.md` & `ape-polygon-0.6.2/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.1/.github/release-drafter.yml` & `ape-polygon-0.6.2/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.1/.github/workflows/commitlint.yaml` & `ape-polygon-0.6.2/.github/workflows/commitlint.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,14 @@
         - uses: actions/checkout@v3
           with:
               fetch-depth: 0
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: pip install commitizen
 
         - name: Check commit history
           run: cz check --rev-range $(git rev-list --all --reverse | head -1)..HEAD
```

### Comparing `ape-polygon-0.6.1/.github/workflows/prtitle.yaml` & `ape-polygon-0.6.2/.github/workflows/prtitle.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: pip install commitizen
 
         - name: Check PR Title
           env:
               TITLE: ${{ github.event.pull_request.title }}
```

### Comparing `ape-polygon-0.6.1/.github/workflows/publish.yaml` & `ape-polygon-0.6.2/.github/workflows/publish.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     steps:
     - uses: actions/checkout@v3
 
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
-        python-version: 3.8
+        python-version: "3.10"
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -e .[release]
         
     - name: Build
```

### Comparing `ape-polygon-0.6.1/.github/workflows/test.yaml` & `ape-polygon-0.6.2/.github/workflows/test.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: pip install .[lint]
 
         - name: Run Black
           run: black --check .
 
@@ -41,15 +41,15 @@
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: pip install .[lint,test]  # Might need test deps
 
         - name: Run MyPy
           run: mypy .
 
@@ -68,16 +68,16 @@
           uses: actions/setup-python@v4
           with:
               python-version: ${{ matrix.python-version }}
 
         - name: Install Dependencies
           run: pip install .[test]
 
-#        - name: Run Tests
-#          run: pytest -m "not fuzzing" -n 0 -s --cov
+        - name: Run Tests
+          run: pytest -m "not fuzzing" -n 0 -s --cov
 
 # NOTE: uncomment this block after you've marked tests with @pytest.mark.fuzzing
 #    fuzzing:
 #        runs-on: ubuntu-latest
 #
 #        strategy:
 #            fail-fast: true
```

### Comparing `ape-polygon-0.6.1/.gitignore` & `ape-polygon-0.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.1/.pre-commit-config.yaml` & `ape-polygon-0.6.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.1/CONTRIBUTING.md` & `ape-polygon-0.6.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.1/LICENSE` & `ape-polygon-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.1/PKG-INFO` & `ape-polygon-0.6.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 Metadata-Version: 2.1
 Name: ape-polygon
-Version: 0.6.1
+Version: 0.6.2
 Summary: ape-polygon: Ape Ecosystem Plugin for Polygon
 Home-page: https://github.com/ApeWorX/ape-polygon
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
-Description: # Quick Start
-        
-        Ecosystem Plugin for Polygon support in Ape
-        
-        ## Dependencies
-        
-        - [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
-        
-        ## Installation
-        
-        ### via `ape`
-        
-        You can install this plugin using `ape`:
-        
-        ```bash
-        ape plugins install polygon
-        ```
-        
-        or via config file:
-        
-        ```yaml
-        # ape-config.yaml
-        plugins:
-          - name: polygon
-        ```
-        
-        ### via `pip`
-        
-        You can install the latest release via [`pip`](https://pypi.org/project/pip/):
-        
-        ```bash
-        pip install ape-polygon
-        ```
-        
-        ### via `setuptools`
-        
-        You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
-        
-        ```bash
-        git clone https://github.com/ApeWorX/ape-polygon.git
-        cd ape-polygon
-        python3 setup.py install
-        ```
-        
-        ## Quick Usage
-        
-        Installing this plugin adds support for the Polygon ecosystem:
-        
-        ```bash
-        ape console --network polygon:mainnet
-        ```
-        
-        ## Development
-        
-        Comments, questions, criticisms and pull requests are welcomed.
-        
 Keywords: ethereum
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8,<3.11
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: release
 Provides-Extra: dev
+License-File: LICENSE
+
+# Quick Start
+
+Ecosystem Plugin for Polygon support in Ape.
+
+## Dependencies
+
+- [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
+
+## Installation
+
+### via `ape`
+
+You can install this plugin using `ape`:
+
+```bash
+ape plugins install polygon
+```
+
+or via config file:
+
+```yaml
+# ape-config.yaml
+plugins:
+  - name: polygon
+```
+
+### via `pip`
+
+You can install the latest release via [`pip`](https://pypi.org/project/pip/):
+
+```bash
+pip install ape-polygon
+```
+
+### via `setuptools`
+
+You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
+
+```bash
+git clone https://github.com/ApeWorX/ape-polygon.git
+cd ape-polygon
+python3 setup.py install
+```
+
+## Quick Usage
+
+Installing this plugin adds support for the Polygon ecosystem:
+
+```bash
+ape console --network polygon:mainnet
+```
+
+## Development
+
+Comments, questions, criticisms and pull requests are welcomed.
```

### Comparing `ape-polygon-0.6.1/README.md` & `ape-polygon-0.6.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Quick Start
 
-Ecosystem Plugin for Polygon support in Ape
+Ecosystem Plugin for Polygon support in Ape.
 
 ## Dependencies
 
 - [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
 
 ## Installation
```

### Comparing `ape-polygon-0.6.1/ape_polygon/__init__.py` & `ape-polygon-0.6.2/ape_polygon/__init__.py`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.1/ape_polygon/ecosystem.py` & `ape-polygon-0.6.2/ape_polygon/ecosystem.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional
+from typing import cast
 
 from ape.api.config import PluginConfig
 from ape.api.networks import LOCAL_NETWORK_NAME
 from ape_ethereum.ecosystem import Ethereum, NetworkConfig
 
 NETWORKS = {
     # chain_id, network_id
@@ -15,26 +15,29 @@
     required_confirmations: int = 1, block_time: int = 2, **kwargs
 ) -> NetworkConfig:
     return NetworkConfig(
         required_confirmations=required_confirmations, block_time=block_time, **kwargs
     )
 
 
-def _create_local_config(default_provider: Optional[str] = None) -> NetworkConfig:
+def _create_local_config() -> NetworkConfig:
     return _create_network_config(
-        required_confirmations=0, block_time=0, default_provider=default_provider
+        required_confirmations=0,
+        block_time=0,
+        default_provider="test",
+        gas_limit="max",
     )
 
 
 class PolygonConfig(PluginConfig):
     mainnet: NetworkConfig = _create_network_config()
     mainnet_fork: NetworkConfig = _create_local_config()
     mumbai: NetworkConfig = _create_network_config()
     mumbai_fork: NetworkConfig = _create_local_config()
-    local: NetworkConfig = NetworkConfig(default_provider="test")
+    local: NetworkConfig = _create_local_config()
     default_network: str = LOCAL_NETWORK_NAME
 
 
 class Polygon(Ethereum):
     @property
-    def config(self) -> PolygonConfig:  # type: ignore
-        return self.config_manager.get_config("polygon")  # type: ignore
+    def config(self) -> PolygonConfig:  # type: ignore[override]
+        return cast(PolygonConfig, self.config_manager.get_config("polygon"))
```

### Comparing `ape-polygon-0.6.1/ape_polygon.egg-info/PKG-INFO` & `ape-polygon-0.6.2/ape_polygon.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 Metadata-Version: 2.1
 Name: ape-polygon
-Version: 0.6.1
+Version: 0.6.2
 Summary: ape-polygon: Ape Ecosystem Plugin for Polygon
 Home-page: https://github.com/ApeWorX/ape-polygon
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
-Description: # Quick Start
-        
-        Ecosystem Plugin for Polygon support in Ape
-        
-        ## Dependencies
-        
-        - [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
-        
-        ## Installation
-        
-        ### via `ape`
-        
-        You can install this plugin using `ape`:
-        
-        ```bash
-        ape plugins install polygon
-        ```
-        
-        or via config file:
-        
-        ```yaml
-        # ape-config.yaml
-        plugins:
-          - name: polygon
-        ```
-        
-        ### via `pip`
-        
-        You can install the latest release via [`pip`](https://pypi.org/project/pip/):
-        
-        ```bash
-        pip install ape-polygon
-        ```
-        
-        ### via `setuptools`
-        
-        You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
-        
-        ```bash
-        git clone https://github.com/ApeWorX/ape-polygon.git
-        cd ape-polygon
-        python3 setup.py install
-        ```
-        
-        ## Quick Usage
-        
-        Installing this plugin adds support for the Polygon ecosystem:
-        
-        ```bash
-        ape console --network polygon:mainnet
-        ```
-        
-        ## Development
-        
-        Comments, questions, criticisms and pull requests are welcomed.
-        
 Keywords: ethereum
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8,<3.11
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: release
 Provides-Extra: dev
+License-File: LICENSE
+
+# Quick Start
+
+Ecosystem Plugin for Polygon support in Ape.
+
+## Dependencies
+
+- [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
+
+## Installation
+
+### via `ape`
+
+You can install this plugin using `ape`:
+
+```bash
+ape plugins install polygon
+```
+
+or via config file:
+
+```yaml
+# ape-config.yaml
+plugins:
+  - name: polygon
+```
+
+### via `pip`
+
+You can install the latest release via [`pip`](https://pypi.org/project/pip/):
+
+```bash
+pip install ape-polygon
+```
+
+### via `setuptools`
+
+You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
+
+```bash
+git clone https://github.com/ApeWorX/ape-polygon.git
+cd ape-polygon
+python3 setup.py install
+```
+
+## Quick Usage
+
+Installing this plugin adds support for the Polygon ecosystem:
+
+```bash
+ape console --network polygon:mainnet
+```
+
+## Development
+
+Comments, questions, criticisms and pull requests are welcomed.
```

### Comparing `ape-polygon-0.6.1/ape_polygon.egg-info/SOURCES.txt` & `ape-polygon-0.6.2/ape_polygon.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -25,9 +25,10 @@
 ape_polygon.egg-info/SOURCES.txt
 ape_polygon.egg-info/dependency_links.txt
 ape_polygon.egg-info/not-zip-safe
 ape_polygon.egg-info/requires.txt
 ape_polygon.egg-info/top_level.txt
 tests/__init__.py
 tests/conftest.py
+tests/test_ecosystem.py
 tests/test_integration.py
 tests/test_provider.py
```

### Comparing `ape-polygon-0.6.1/ape_polygon.egg-info/requires.txt` & `ape-polygon-0.6.2/ape_polygon.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 eth-ape<0.7,>=0.6.0
+typing-extensions==4.5.0
 
 [dev]
 pytest>=6.0
 pytest-xdist
 pytest-cov
 hypothesis<7,>=6.2.0
 black<24,>=23.3.0
```

### Comparing `ape-polygon-0.6.1/pyproject.toml` & `ape-polygon-0.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.1/setup.py` & `ape-polygon-0.6.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -54,16 +54,17 @@
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-polygon",
     include_package_data=True,
     install_requires=[
         "eth-ape>=0.6.0,<0.7",
+        "typing-extensions==4.5.0",  # Can remove once Pydantic patched and ape updated.
     ],
-    python_requires=">=3.8,<3.11",
+    python_requires=">=3.8,<4",
     extras_require=extras_require,
     py_modules=["ape_polygon"],
     license="Apache-2.0",
     zip_safe=False,
     keywords="ethereum",
     packages=find_packages(exclude=["tests", "tests.*"]),
     package_data={"ape_polygon": ["py.typed"]},
@@ -74,9 +75,10 @@
         "Natural Language :: English",
         "Operating System :: MacOS",
         "Operating System :: POSIX",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

### Comparing `ape-polygon-0.6.1/tests/test_integration.py` & `ape-polygon-0.6.2/tests/test_integration.py`

 * *Files identical despite different names*

