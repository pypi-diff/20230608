# Comparing `tmp/pypistats-1.3.0.tar.gz` & `tmp/pypistats-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, last modified: Thu Jun  8 14:02:38 2023, max compression
```

## Comparing `pypistats-1.3.0.tar` & `pypistats-1.4.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 pypistats-1.3.0/.coveragerc
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 pypistats-1.3.0/.editorconfig
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 pypistats-1.3.0/.flake8
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 pypistats-1.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 pypistats-1.3.0/RELEASING.md
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 pypistats-1.3.0/azure-pipelines.yml
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 pypistats-1.3.0/requirements.txt
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 pypistats-1.3.0/tox.ini
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 pypistats-1.3.0/.azure-pipelines/jobs/lint.yml
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 pypistats-1.3.0/.azure-pipelines/jobs/test.yml
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 pypistats-1.3.0/.github/labels.yml
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 pypistats-1.3.0/.github/release-drafter.yml
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 pypistats-1.3.0/.github/renovate.json
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 pypistats-1.3.0/.github/workflows/deploy.yml
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 pypistats-1.3.0/.github/workflows/labels.yml
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 pypistats-1.3.0/.github/workflows/lint.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pypistats-1.3.0/.github/workflows/release-drafter.yml
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 pypistats-1.3.0/.github/workflows/require-pr-label.yml
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 pypistats-1.3.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 pypistats-1.3.0/example/example.py
--rw-r--r--   0        0        0    45231 2020-02-02 00:00:00.000000 pypistats-1.3.0/example/overall.png
--rw-r--r--   0        0        0    43322 2020-02-02 00:00:00.000000 pypistats-1.3.0/example/python3.png
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 pypistats-1.3.0/scripts/run_command.py
--rw-r--r--   0        0        0    14380 2020-02-02 00:00:00.000000 pypistats-1.3.0/src/pypistats/__init__.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 pypistats-1.3.0/src/pypistats/__main__.py
--rw-r--r--   0        0        0     9615 2020-02-02 00:00:00.000000 pypistats-1.3.0/src/pypistats/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypistats-1.3.0/tests/__init__.py
--rw-r--r--   0        0        0     4729 2020-02-02 00:00:00.000000 pypistats-1.3.0/tests/test_cli.py
--rw-r--r--   0        0        0    24904 2020-02-02 00:00:00.000000 pypistats-1.3.0/tests/test_pypistats.py
--rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 pypistats-1.3.0/tests/test_pypistats_cache.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 pypistats-1.3.0/tests/test_pypistats_print.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypistats-1.3.0/tests/data/__init__.py
--rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 pypistats-1.3.0/tests/data/expected_tabulated.py
--rw-r--r--   0        0        0    93203 2020-02-02 00:00:00.000000 pypistats-1.3.0/tests/data/python_minor.py
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 pypistats-1.3.0/.gitignore
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pypistats-1.3.0/LICENSE.txt
--rw-r--r--   0        0        0    12457 2020-02-02 00:00:00.000000 pypistats-1.3.0/README.md
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 pypistats-1.3.0/pyproject.toml
--rw-r--r--   0        0        0    14338 2020-02-02 00:00:00.000000 pypistats-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      320 2023-06-08 14:02:38.000000 pypistats-1.4.0/.coveragerc
+-rw-r--r--   0        0        0      371 2023-06-08 14:02:38.000000 pypistats-1.4.0/.editorconfig
+-rw-r--r--   0        0        0       30 2023-06-08 14:02:38.000000 pypistats-1.4.0/.flake8
+-rw-r--r--   0        0        0     1467 2023-06-08 14:02:38.000000 pypistats-1.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      830 2023-06-08 14:02:38.000000 pypistats-1.4.0/RELEASING.md
+-rw-r--r--   0        0        0     1168 2023-06-08 14:02:38.000000 pypistats-1.4.0/azure-pipelines.yml
+-rw-r--r--   0        0        0      256 2023-06-08 14:02:38.000000 pypistats-1.4.0/requirements.txt
+-rw-r--r--   0        0        0      755 2023-06-08 14:02:38.000000 pypistats-1.4.0/tox.ini
+-rw-r--r--   0        0        0      647 2023-06-08 14:02:38.000000 pypistats-1.4.0/.azure-pipelines/jobs/lint.yml
+-rw-r--r--   0        0        0     1069 2023-06-08 14:02:38.000000 pypistats-1.4.0/.azure-pipelines/jobs/test.yml
+-rw-r--r--   0        0        0     1785 2023-06-08 14:02:38.000000 pypistats-1.4.0/.github/labels.yml
+-rw-r--r--   0        0        0      892 2023-06-08 14:02:38.000000 pypistats-1.4.0/.github/release-drafter.yml
+-rw-r--r--   0        0        0      443 2023-06-08 14:02:38.000000 pypistats-1.4.0/.github/renovate.json
+-rw-r--r--   0        0        0     1755 2023-06-08 14:02:38.000000 pypistats-1.4.0/.github/workflows/deploy.yml
+-rw-r--r--   0        0        0      352 2023-06-08 14:02:38.000000 pypistats-1.4.0/.github/workflows/labels.yml
+-rw-r--r--   0        0        0      298 2023-06-08 14:02:38.000000 pypistats-1.4.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1084 2023-06-08 14:02:38.000000 pypistats-1.4.0/.github/workflows/release-drafter.yml
+-rw-r--r--   0        0        0      490 2023-06-08 14:02:38.000000 pypistats-1.4.0/.github/workflows/require-pr-label.yml
+-rw-r--r--   0        0        0     1332 2023-06-08 14:02:38.000000 pypistats-1.4.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1673 2023-06-08 14:02:38.000000 pypistats-1.4.0/example/example.py
+-rw-r--r--   0        0        0    45231 2023-06-08 14:02:38.000000 pypistats-1.4.0/example/overall.png
+-rw-r--r--   0        0        0    43322 2023-06-08 14:02:38.000000 pypistats-1.4.0/example/python3.png
+-rw-r--r--   0        0        0      333 2023-06-08 14:02:38.000000 pypistats-1.4.0/scripts/run_command.py
+-rw-r--r--   0        0        0    14307 2023-06-08 14:02:38.000000 pypistats-1.4.0/src/pypistats/__init__.py
+-rw-r--r--   0        0        0      105 2023-06-08 14:02:38.000000 pypistats-1.4.0/src/pypistats/__main__.py
+-rw-r--r--   0        0        0     9615 2023-06-08 14:02:38.000000 pypistats-1.4.0/src/pypistats/cli.py
+-rw-r--r--   0        0        0        0 2023-06-08 14:02:38.000000 pypistats-1.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     4729 2023-06-08 14:02:38.000000 pypistats-1.4.0/tests/test_cli.py
+-rw-r--r--   0        0        0    24904 2023-06-08 14:02:38.000000 pypistats-1.4.0/tests/test_pypistats.py
+-rw-r--r--   0        0        0     3037 2023-06-08 14:02:38.000000 pypistats-1.4.0/tests/test_pypistats_cache.py
+-rw-r--r--   0        0        0      308 2023-06-08 14:02:38.000000 pypistats-1.4.0/tests/test_pypistats_print.py
+-rw-r--r--   0        0        0        0 2023-06-08 14:02:38.000000 pypistats-1.4.0/tests/data/__init__.py
+-rw-r--r--   0        0        0     4080 2023-06-08 14:02:38.000000 pypistats-1.4.0/tests/data/expected_tabulated.py
+-rw-r--r--   0        0        0    93203 2023-06-08 14:02:38.000000 pypistats-1.4.0/tests/data/python_minor.py
+-rw-r--r--   0        0        0     1298 2023-06-08 14:02:38.000000 pypistats-1.4.0/.gitignore
+-rw-r--r--   0        0        0     1079 2023-06-08 14:02:38.000000 pypistats-1.4.0/LICENSE.txt
+-rw-r--r--   0        0        0    12457 2023-06-08 14:02:38.000000 pypistats-1.4.0/README.md
+-rw-r--r--   0        0        0     1818 2023-06-08 14:02:38.000000 pypistats-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0    14230 2023-06-08 14:02:38.000000 pypistats-1.4.0/PKG-INFO
```

### Comparing `pypistats-1.3.0/.pre-commit-config.yaml` & `pypistats-1.4.0/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,62 +1,64 @@
 repos:
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.1
+    rev: v3.4.0
     hooks:
       - id: pyupgrade
-        args: [--py37-plus]
+        args: [--py38-plus]
 
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/PyCQA/isort
     rev: 5.12.0
     hooks:
       - id: isort
 
   - repo: https://github.com/PyCQA/flake8
     rev: 6.0.0
     hooks:
       - id: flake8
-        additional_dependencies: [flake8-2020, flake8-implicit-str-concat]
+        additional_dependencies:
+          [flake8-2020, flake8-errmsg, flake8-implicit-str-concat]
 
   - repo: https://github.com/pre-commit/pygrep-hooks
     rev: v1.10.0
     hooks:
       - id: python-check-blanket-noqa
       - id: python-no-log-warn
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
-      - id: check-json
+      - id: check-case-conflict
       - id: check-merge-conflict
+      - id: check-json
       - id: check-toml
       - id: check-yaml
       - id: end-of-file-fixer
       - id: requirements-txt-fixer
 
   - repo: https://github.com/tox-dev/pyproject-fmt
-    rev: 0.6.0
+    rev: 0.10.0
     hooks:
       - id: pyproject-fmt
 
   - repo: https://github.com/abravalheri/validate-pyproject
-    rev: v0.12.1
+    rev: v0.13
     hooks:
       - id: validate-pyproject
 
   - repo: https://github.com/tox-dev/tox-ini-fmt
-    rev: 0.6.1
+    rev: 1.3.0
     hooks:
       - id: tox-ini-fmt
 
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v3.0.0-alpha.4
+    rev: v3.0.0-alpha.9-for-vscode
     hooks:
       - id: prettier
         args: [--prose-wrap=always, --print-width=88]
 
 ci:
   autoupdate_schedule: quarterly
```

### Comparing `pypistats-1.3.0/RELEASING.md` & `pypistats-1.4.0/RELEASING.md`

 * *Files identical despite different names*

### Comparing `pypistats-1.3.0/azure-pipelines.yml` & `pypistats-1.4.0/azure-pipelines.yml`

 * *Files identical despite different names*

### Comparing `pypistats-1.3.0/tox.ini` & `pypistats-1.4.0/tox.ini`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 [tox]
-envlist =
+requires =
+    tox>=4.2
+env_list =
     cog
     lint
     pins
-    py{py3, 312, 311, 310, 39, 38, 37}
+    py{py3, 312, 311, 310, 39, 38}
 
 [testenv]
 extras =
     tests
+commands_pre =
+    - {envpython} -m pip install --only-binary :all: numpy pandas
 commands =
     {envpython} -m pytest --cov pypistats --cov tests --cov-report html --cov-report term --cov-report xml {posargs}
     pypistats --version
     pypistats --help
     pypistats recent --help
-commands_pre =
-    - {envpython} -m pip install --only-binary :all: numpy pandas
 
 [testenv:cog]
 skip_install = true
 deps =
     cogapp
 commands =
     cog -Pr README.md
 
 [testenv:lint]
-passenv =
-    PRE_COMMIT_COLOR
 skip_install = true
 deps =
     pre-commit
+pass_env =
+    PRE_COMMIT_COLOR
 commands =
     pre-commit run --all-files --show-diff-on-failure
 
 [testenv:pins]
 extras =
     None
 commands_pre =
```

### Comparing `pypistats-1.3.0/.azure-pipelines/jobs/lint.yml` & `pypistats-1.4.0/.azure-pipelines/jobs/lint.yml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 jobs:
   - job: ${{ parameters.name }}
     pool:
       vmImage: ${{ parameters.vmImage }}
 
     strategy:
       matrix:
-        Python37:
+        Python311:
           python.version: "3.11"
 
     steps:
       - task: UsePythonVersion@0.206.0
         inputs:
           versionSpec: "$(python.version)"
           architecture: "x64"
```

### Comparing `pypistats-1.3.0/.azure-pipelines/jobs/test.yml` & `pypistats-1.4.0/.azure-pipelines/jobs/test.yml`

 * *Files 23% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 jobs:
   - job: ${{ parameters.name }}
     pool:
       vmImage: ${{ parameters.vmImage }}
 
     strategy:
       matrix:
-        Python37:
-          python.version: "3.7"
         Python38:
           python.version: "3.8"
         Python39:
           python.version: "3.9"
         Python310:
           python.version: "3.10"
         Python311:
@@ -36,13 +34,7 @@
           pytest --cov pypistats --cov-report html --test-run-title="${{ parameters.name }} Python $(python.version)"
         displayName: "Unit tests"
 
       - script: |
           pypistats --help
           pypistats recent --help
         displayName: "Test runs"
-
-      - script: |
-          python -m pip install --upgrade codecov
-          codecov --name "Azure: ${{ parameters.name }} Python $(python.version)" --build $(Build.BuildNumber) --token $(CODECOV_TOKEN)
-        condition: succeeded()
-        displayName: "Upload to Codecov"
```

### Comparing `pypistats-1.3.0/.github/labels.yml` & `pypistats-1.4.0/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `pypistats-1.3.0/.github/release-drafter.yml` & `pypistats-1.4.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `pypistats-1.3.0/.github/workflows/release-drafter.yml` & `pypistats-1.4.0/.github/workflows/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `pypistats-1.3.0/.github/workflows/test.yml` & `pypistats-1.4.0/.github/workflows/test.yml`

 * *Files 11% similar despite different names*

```diff
@@ -7,24 +7,25 @@
 
 jobs:
   test:
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["pypy3.9", "3.7", "3.8", "3.9", "3.10", "3.11", "3.12-dev"]
+        python-version: ["pypy3.9", "3.8", "3.9", "3.10", "3.11", "3.12"]
         os: [windows-latest, macos-latest, ubuntu-latest]
 
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
+          allow-prereleases: true
           cache: pip
           cache-dependency-path: pyproject.toml
 
       - name: Install dependencies
         run: |
           python -m pip install -U pip
           python -m pip install -U wheel
```

### Comparing `pypistats-1.3.0/example/example.py` & `pypistats-1.4.0/example/example.py`

 * *Files identical despite different names*

### Comparing `pypistats-1.3.0/example/overall.png` & `pypistats-1.4.0/example/overall.png`

 * *Files identical despite different names*

### Comparing `pypistats-1.3.0/example/python3.png` & `pypistats-1.4.0/example/python3.png`

 * *Files identical despite different names*

### Comparing `pypistats-1.3.0/src/pypistats/__init__.py` & `pypistats-1.4.0/src/pypistats/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,31 +2,25 @@
 Python interface to PyPI Stats API
 https://pypistats.org/api
 """
 from __future__ import annotations
 
 import atexit
 import datetime as dt
+import importlib.metadata
 import json
 import sys
 import warnings
 from pathlib import Path
 
 from platformdirs import user_cache_dir
 from slugify import slugify
 from termcolor import colored
 
-try:
-    # Python 3.8+
-    import importlib.metadata as importlib_metadata
-except ImportError:
-    # Python 3.7
-    import importlib_metadata
-
-__version__ = importlib_metadata.version(__name__)
+__version__ = importlib.metadata.version(__name__)
 
 BASE_URL = "https://pypistats.org/api/"
 CACHE_DIR = Path(user_cache_dir("pypistats"))
 USER_AGENT = f"pypistats/{__version__}"
 
 
 def _print_verbose(verbose: bool, *args, **kwargs) -> None:
@@ -38,15 +32,15 @@
 def _print_stderr(*args, **kwargs) -> None:
     """Print to stderr"""
     print(*args, file=sys.stderr, **kwargs)
 
 
 def _cache_filename(url: str) -> Path:
     """yyyy-mm-dd-url-slug.json"""
-    today = dt.datetime.utcnow().strftime("%Y-%m-%d")
+    today = dt.datetime.now(dt.timezone.utc).strftime("%Y-%m-%d")
     slug = slugify(url)
     filename = CACHE_DIR / f"{today}-{slug}.json"
 
     return filename
 
 
 def _load_cache(cache_file: Path) -> dict:
@@ -73,15 +67,15 @@
     except OSError:
         pass
 
 
 def _clear_cache() -> None:
     """Delete old cache files, run as last task"""
     cache_files = CACHE_DIR.glob("**/*.json")
-    this_month = dt.datetime.utcnow().strftime("%Y-%m")
+    this_month = dt.datetime.now(dt.timezone.utc).strftime("%Y-%m")
     for cache_file in cache_files:
         if not cache_file.name.startswith(this_month):
             cache_file.unlink()
 
 
 atexit.register(_clear_cache)
 
@@ -130,19 +124,20 @@
         _save_cache(cache_file, res)
 
     # Actual first and last dates of the fetched data
     first, last = _date_range(res["data"])
 
     # Validate end date
     if end_date and end_date < first:
-        raise ValueError(
+        msg = (
             f"Requested end date ({end_date}) is before earliest available "
             f"data ({first}), because data is only available for 180 days. "
             "See https://pypistats.org/about#data"
         )
+        raise ValueError(msg)
 
     # Validate start date
     if start_date and start_date < first:
         warnings.warn(
             f"Requested start date ({start_date}) is before earliest available "
             f"data ({first}), because data is only available for 180 days. "
             "See https://pypistats.org/about#data",
```

### Comparing `pypistats-1.3.0/src/pypistats/cli.py` & `pypistats-1.4.0/src/pypistats/cli.py`

 * *Files identical despite different names*

### Comparing `pypistats-1.3.0/tests/test_cli.py` & `pypistats-1.4.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pypistats-1.3.0/tests/test_pypistats.py` & `pypistats-1.4.0/tests/test_pypistats.py`

 * *Files identical despite different names*

### Comparing `pypistats-1.3.0/tests/test_pypistats_cache.py` & `pypistats-1.4.0/tests/test_pypistats_cache.py`

 * *Files identical despite different names*

### Comparing `pypistats-1.3.0/tests/data/expected_tabulated.py` & `pypistats-1.4.0/tests/data/expected_tabulated.py`

 * *Files identical despite different names*

### Comparing `pypistats-1.3.0/tests/data/python_minor.py` & `pypistats-1.4.0/tests/data/python_minor.py`

 * *Files identical despite different names*

### Comparing `pypistats-1.3.0/.gitignore` & `pypistats-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pypistats-1.3.0/LICENSE.txt` & `pypistats-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pypistats-1.3.0/README.md` & `pypistats-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pypistats-1.3.0/pyproject.toml` & `pypistats-1.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -14,38 +14,36 @@
   "downloads",
   "PyPI",
   "statistics",
   "stats",
 ]
 license = {text = "MIT"}
 authors = [{name = "Hugo van Kemenade"}]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 classifiers = [
-    "Development Status :: 5 - Production/Stable",
-    "Intended Audience :: Developers",
-    "Intended Audience :: End Users/Desktop",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3.12",
-    "Programming Language :: Python :: Implementation :: CPython",
-    "Programming Language :: Python :: Implementation :: PyPy",
+  "Development Status :: 5 - Production/Stable",
+  "Intended Audience :: Developers",
+  "Intended Audience :: End Users/Desktop",
+  "License :: OSI Approved :: MIT License",
+  "Operating System :: OS Independent",
+  "Programming Language :: Python :: 3",
+  "Programming Language :: Python :: 3 :: Only",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
+  "Programming Language :: Python :: Implementation :: CPython",
+  "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dynamic = [
   "version",
 ]
 dependencies = [
   "httpx>=0.19",
-  'importlib-metadata; python_version < "3.8"',
   "platformdirs",
   "prettytable>=2.4",
   "pytablewriter[html]>=0.63",
   "python-dateutil",
   "python-slugify",
   "termcolor>=2.1",
 ]
@@ -58,24 +56,21 @@
 ]
 tests = [
   "freezegun",
   "pytest",
   "pytest-cov",
   "respx>=0.11",
 ]
-
 [project.urls]
 Changelog = "https://github.com/hugovk/pypistats/releases"
 Homepage = "https://github.com/hugovk/pypistats"
 Source = "https://github.com/hugovk/pypistats"
-
 [project.scripts]
 pypistats = "pypistats.cli:main"
 
-
 [tool.hatch]
 version.source = "vcs"
 
 [tool.hatch.version.raw-options]
 local_scheme = "no-local-version"
 
 [tool.isort]
```

### Comparing `pypistats-1.3.0/PKG-INFO` & `pypistats-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypistats
-Version: 1.3.0
+Version: 1.4.0
 Summary: Python interface to PyPI Stats API https://pypistats.org/api
 Project-URL: Changelog, https://github.com/hugovk/pypistats/releases
 Project-URL: Homepage, https://github.com/hugovk/pypistats
 Project-URL: Source, https://github.com/hugovk/pypistats
 Author: Hugo van Kemenade
 License: MIT
 License-File: LICENSE.txt
@@ -12,25 +12,23 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: httpx>=0.19
-Requires-Dist: importlib-metadata; python_version < '3.8'
 Requires-Dist: platformdirs
 Requires-Dist: prettytable>=2.4
 Requires-Dist: pytablewriter[html]>=0.63
 Requires-Dist: python-dateutil
 Requires-Dist: python-slugify
 Requires-Dist: termcolor>=2.1
 Provides-Extra: numpy
```

