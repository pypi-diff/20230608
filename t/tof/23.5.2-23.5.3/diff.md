# Comparing `tmp/tof-23.5.2.tar.gz` & `tmp/tof-23.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tof-23.5.2.tar", last modified: Mon May 22 11:45:28 2023, max compression
+gzip compressed data, was "tof-23.5.3.tar", last modified: Thu Jun  8 09:16:16 2023, max compression
```

## Comparing `tof-23.5.2.tar` & `tof-23.5.3.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:45:28.477793 tof-23.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-22 11:45:16.000000 tof-23.5.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:45:28.469793 tof-23.5.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:45:28.473793 tof-23.5.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-22 11:45:16.000000 tof-23.5.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-22 11:45:16.000000 tof-23.5.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-22 11:45:16.000000 tof-23.5.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-22 11:45:16.000000 tof-23.5.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-22 11:45:16.000000 tof-23.5.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-22 11:45:16.000000 tof-23.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-05-22 11:45:28.477793 tof-23.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-05-22 11:45:16.000000 tof-23.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:45:28.473793 tof-23.5.2/conda/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-22 11:45:16.000000 tof-23.5.2/conda/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:45:28.473793 tof-23.5.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:45:28.473793 tof-23.5.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    22254 2023-05-22 11:45:16.000000 tof-23.5.2/docs/_static/detector.png
--rw-r--r--   0 runner    (1001) docker     (123)   137750 2023-05-22 11:45:16.000000 tof-23.5.2/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-05-22 11:45:16.000000 tof-23.5.2/docs/_static/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    96012 2023-05-22 11:45:16.000000 tof-23.5.2/docs/_static/model.png
--rw-r--r--   0 runner    (1001) docker     (123)    32531 2023-05-22 11:45:16.000000 tof-23.5.2/docs/_static/pulse.png
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-22 11:45:16.000000 tof-23.5.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9534 2023-05-22 11:45:16.000000 tof-23.5.2/docs/components.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-22 11:45:16.000000 tof-23.5.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-22 11:45:16.000000 tof-23.5.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-05-22 11:45:16.000000 tof-23.5.2/docs/multiple-pulses.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-22 11:45:16.000000 tof-23.5.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9817 2023-05-22 11:45:16.000000 tof-23.5.2/docs/short-example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-05-22 11:45:16.000000 tof-23.5.2/docs/sources.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-22 11:45:16.000000 tof-23.5.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:45:28.477793 tof-23.5.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-22 11:45:16.000000 tof-23.5.2/requirements/ci.in
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-22 11:45:16.000000 tof-23.5.2/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-22 11:45:16.000000 tof-23.5.2/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-05-22 11:45:16.000000 tof-23.5.2/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-22 11:45:16.000000 tof-23.5.2/requirements/static.in
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-22 11:45:16.000000 tof-23.5.2/requirements/static.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-22 11:45:16.000000 tof-23.5.2/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-22 11:45:16.000000 tof-23.5.2/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-22 11:45:16.000000 tof-23.5.2/requirements/wheels.in
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-22 11:45:16.000000 tof-23.5.2/requirements/wheels.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 11:45:28.477793 tof-23.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:45:28.469793 tof-23.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:45:28.473793 tof-23.5.2/src/tof/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-22 11:45:16.000000 tof-23.5.2/src/tof/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-05-22 11:45:16.000000 tof-23.5.2/src/tof/chopper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-05-22 11:45:16.000000 tof-23.5.2/src/tof/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-22 11:45:16.000000 tof-23.5.2/src/tof/detector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:45:28.473793 tof-23.5.2/src/tof/facilities/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-22 11:45:16.000000 tof-23.5.2/src/tof/facilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21295 2023-05-22 11:45:16.000000 tof-23.5.2/src/tof/facilities/ess_pulse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-05-22 11:45:16.000000 tof-23.5.2/src/tof/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12783 2023-05-22 11:45:16.000000 tof-23.5.2/src/tof/result.py
--rw-r--r--   0 runner    (1001) docker     (123)    12592 2023-05-22 11:45:16.000000 tof-23.5.2/src/tof/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-22 11:45:16.000000 tof-23.5.2/src/tof/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:45:28.473793 tof-23.5.2/src/tof.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-05-22 11:45:28.000000 tof-23.5.2/src/tof.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-22 11:45:28.000000 tof-23.5.2/src/tof.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 11:45:28.000000 tof-23.5.2/src/tof.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 11:45:28.000000 tof-23.5.2/src/tof.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-22 11:45:28.000000 tof-23.5.2/src/tof.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:45:28.477793 tof-23.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-22 11:45:16.000000 tof-23.5.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-05-22 11:45:16.000000 tof-23.5.2/tests/chopper_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-22 11:45:16.000000 tof-23.5.2/tests/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    10958 2023-05-22 11:45:16.000000 tof-23.5.2/tests/model_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-05-22 11:45:16.000000 tof-23.5.2/tests/result_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8914 2023-05-22 11:45:16.000000 tof-23.5.2/tests/source_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-22 11:45:16.000000 tof-23.5.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:16:16.578825 tof-23.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-08 09:16:02.000000 tof-23.5.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:16:16.566825 tof-23.5.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:16:16.570825 tof-23.5.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-08 09:16:02.000000 tof-23.5.3/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-06-08 09:16:02.000000 tof-23.5.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-08 09:16:02.000000 tof-23.5.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-08 09:16:02.000000 tof-23.5.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-08 09:16:02.000000 tof-23.5.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-08 09:16:02.000000 tof-23.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-06-08 09:16:16.578825 tof-23.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-08 09:16:02.000000 tof-23.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:16:16.570825 tof-23.5.3/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-08 09:16:02.000000 tof-23.5.3/conda/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:16:16.574825 tof-23.5.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:16:16.574825 tof-23.5.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    22254 2023-06-08 09:16:02.000000 tof-23.5.3/docs/_static/detector.png
+-rw-r--r--   0 runner    (1001) docker     (123)   137750 2023-06-08 09:16:02.000000 tof-23.5.3/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-06-08 09:16:02.000000 tof-23.5.3/docs/_static/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    96012 2023-06-08 09:16:02.000000 tof-23.5.3/docs/_static/model.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32531 2023-06-08 09:16:02.000000 tof-23.5.3/docs/_static/pulse.png
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-08 09:16:02.000000 tof-23.5.3/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9534 2023-06-08 09:16:02.000000 tof-23.5.3/docs/components.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-06-08 09:16:02.000000 tof-23.5.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-08 09:16:02.000000 tof-23.5.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-06-08 09:16:02.000000 tof-23.5.3/docs/multiple-pulses.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-08 09:16:02.000000 tof-23.5.3/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9817 2023-06-08 09:16:02.000000 tof-23.5.3/docs/short-example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-06-08 09:16:02.000000 tof-23.5.3/docs/sources.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-08 09:16:02.000000 tof-23.5.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:16:16.574825 tof-23.5.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-08 09:16:02.000000 tof-23.5.3/requirements/ci.in
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-08 09:16:02.000000 tof-23.5.3/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-08 09:16:02.000000 tof-23.5.3/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-06-08 09:16:02.000000 tof-23.5.3/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-08 09:16:02.000000 tof-23.5.3/requirements/static.in
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-08 09:16:02.000000 tof-23.5.3/requirements/static.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 09:16:02.000000 tof-23.5.3/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-08 09:16:02.000000 tof-23.5.3/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-08 09:16:02.000000 tof-23.5.3/requirements/wheels.in
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-08 09:16:02.000000 tof-23.5.3/requirements/wheels.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 09:16:16.578825 tof-23.5.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:16:16.566825 tof-23.5.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:16:16.570825 tof-23.5.3/src/tof/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-08 09:16:02.000000 tof-23.5.3/src/tof/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-06-08 09:16:02.000000 tof-23.5.3/src/tof/chopper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-06-08 09:16:02.000000 tof-23.5.3/src/tof/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-08 09:16:02.000000 tof-23.5.3/src/tof/detector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:16:16.570825 tof-23.5.3/src/tof/facilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-08 09:16:02.000000 tof-23.5.3/src/tof/facilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21295 2023-06-08 09:16:02.000000 tof-23.5.3/src/tof/facilities/ess_pulse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-06-08 09:16:02.000000 tof-23.5.3/src/tof/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12819 2023-06-08 09:16:02.000000 tof-23.5.3/src/tof/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12592 2023-06-08 09:16:02.000000 tof-23.5.3/src/tof/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-08 09:16:02.000000 tof-23.5.3/src/tof/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:16:16.570825 tof-23.5.3/src/tof.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-06-08 09:16:16.000000 tof-23.5.3/src/tof.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-08 09:16:16.000000 tof-23.5.3/src/tof.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 09:16:16.000000 tof-23.5.3/src/tof.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 09:16:16.000000 tof-23.5.3/src/tof.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-08 09:16:16.000000 tof-23.5.3/src/tof.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:16:16.578825 tof-23.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-08 09:16:02.000000 tof-23.5.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-06-08 09:16:02.000000 tof-23.5.3/tests/chopper_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-08 09:16:02.000000 tof-23.5.3/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10958 2023-06-08 09:16:02.000000 tof-23.5.3/tests/model_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-06-08 09:16:02.000000 tof-23.5.3/tests/result_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8914 2023-06-08 09:16:02.000000 tof-23.5.3/tests/source_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-08 09:16:02.000000 tof-23.5.3/tox.ini
```

### Comparing `tof-23.5.2/.github/workflows/ci.yml` & `tof-23.5.3/.github/workflows/ci.yml`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,15 @@
   formatting:
     name: Formatting and static analysis
     runs-on: ubuntu-22.04
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v3
         with:
-          python-version: '3.10'
+          python-version: '3.8'
       - run: python -m pip install --upgrade pip
       - run: python -m pip install -r requirements/ci.txt
       - run: tox -e static
       - uses: stefanzweifel/git-auto-commit-action@v4
         with:
           commit_message: Apply automatic formatting
 
@@ -33,29 +33,29 @@
     name: Tests
     needs: formatting
     runs-on: ubuntu-22.04
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v3
         with:
-          python-version: '3.10'
+          python-version: '3.8'
       - run: python -m pip install --upgrade pip
       - run: python -m pip install -r requirements/ci.txt
       - run: tox
 
   docs:
     needs: tests
     name: Documentation
     runs-on: ubuntu-22.04
     steps:
       - run: sudo apt install --yes pandoc
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v3
         with:
-          python-version: '3.10'
+          python-version: '3.8'
       - run: python -m pip install --upgrade pip
       - run: python -m pip install -r requirements/ci.txt
       - run: tox -e docs
       - uses: actions/upload-artifact@v3
         with:
           name: html
           path: html/
```

### Comparing `tof-23.5.2/.github/workflows/release.yml` & `tof-23.5.3/.github/workflows/release.yml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
       - uses: actions/checkout@v3
         with:
           submodules: true
           fetch-depth: 0  # history required so cmake can determine version
 
       - uses: conda-incubator/setup-miniconda@v2
       - run: conda install -c conda-forge --yes conda-build boa
-      - run: conda mambabuild --channel conda-forge --channel scipp --python=3.10 --no-anaconda-upload --override-channels --output-folder conda/package conda
+      - run: conda mambabuild --channel conda-forge --channel scipp --python=3.8 --no-anaconda-upload --override-channels --output-folder conda/package conda
 
       - uses: actions/upload-artifact@v3
         with:
           name: conda-package-noarch
           path: conda/package/*/tof*.tar.bz2
 
   build_wheels:
@@ -39,15 +39,15 @@
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0  # history required so setuptools_scm can determine version
 
       - uses: actions/setup-python@v3
         with:
-          python-version: '3.10'
+          python-version: '3.8'
 
       - run: python -m pip install --upgrade pip
       - run: python -m pip install -r requirements/wheels.txt
 
       - name: Build wheels
         run: python -m build
```

### Comparing `tof-23.5.2/.pre-commit-config.yaml` & `tof-23.5.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `tof-23.5.2/LICENSE` & `tof-23.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tof-23.5.2/PKG-INFO` & `tof-23.5.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tof
-Version: 23.5.2
+Version: 23.5.3
 Summary: A simple tool to create time-of-flight chopper cascade diagrams
 Author: Neil Vaytet
 License: BSD-3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -14,14 +14,20 @@
 
 [![Documentation Status](https://readthedocs.org/projects/tof/badge/?version=latest)](https://tof.readthedocs.io/en/latest/?badge=latest)
 
 # tof
 
 A simple tool to create time-of-flight chopper cascade diagrams
 
+**Scope:**
+
+- ``tof`` is designed to be simple and lightweight, it will never replace [McStas](https://www.mcstas.org/)
+- it assumes all neutrons travel in a straight line
+- it does not simulate absorption or scattering effects
+
 ## Installation
 
 ```sh
 pip install tof
 ```
 
 ## Documentation
```

### Comparing `tof-23.5.2/README.md` & `tof-23.5.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 [![Documentation Status](https://readthedocs.org/projects/tof/badge/?version=latest)](https://tof.readthedocs.io/en/latest/?badge=latest)
 
 # tof
 
 A simple tool to create time-of-flight chopper cascade diagrams
 
+**Scope:**
+
+- ``tof`` is designed to be simple and lightweight, it will never replace [McStas](https://www.mcstas.org/)
+- it assumes all neutrons travel in a straight line
+- it does not simulate absorption or scattering effects
+
 ## Installation
 
 ```sh
 pip install tof
 ```
 
 ## Documentation
```

### Comparing `tof-23.5.2/conda/meta.yaml` & `tof-23.5.3/conda/meta.yaml`

 * *Files identical despite different names*

### Comparing `tof-23.5.2/docs/_static/detector.png` & `tof-23.5.3/docs/_static/detector.png`

 * *Files identical despite different names*

### Comparing `tof-23.5.2/docs/_static/favicon.ico` & `tof-23.5.3/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tof-23.5.2/docs/_static/logo.svg` & `tof-23.5.3/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `tof-23.5.2/docs/_static/model.png` & `tof-23.5.3/docs/_static/model.png`

 * *Files identical despite different names*

### Comparing `tof-23.5.2/docs/_static/pulse.png` & `tof-23.5.3/docs/_static/pulse.png`

 * *Files identical despite different names*

### Comparing `tof-23.5.2/docs/components.ipynb` & `tof-23.5.3/docs/components.ipynb`

 * *Files identical despite different names*

### Comparing `tof-23.5.2/docs/conf.py` & `tof-23.5.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tof-23.5.2/docs/index.rst` & `tof-23.5.3/docs/index.rst`

 * *Files 20% similar despite different names*

```diff
@@ -8,14 +8,20 @@
 .. role:: transparent
 
 :transparent:`Tof`
 ******************
 
 A simple tool to create time-of-flight chopper cascade diagrams.
 
+**Scope:**
+
+* ``tof`` is designed to be simple and lightweight, it will never replace `McStas <https://www.mcstas.org/>`_
+* it assumes all neutrons travel in a straight line
+* it does not simulate absorption or scattering effects
+
 Installation
 ============
 
 You can install from ``pip`` using
 
 .. code-block:: sh
```

#### html2text {}

```diff
@@ -1,9 +1,12 @@
 .. raw:: html
 [_static/logo.svg]
  .. role:: transparent :transparent:`Tof` ****************** A simple tool to
-create time-of-flight chopper cascade diagrams. Installation ============ You
-can install from ``pip`` using .. code-block:: sh pip install tof You can
+create time-of-flight chopper cascade diagrams. **Scope:** * ``tof`` is
+designed to be simple and lightweight, it will never replace `McStas
+www.mcstas.org/>`_ * it assumes all neutrons travel in a straight line * it
+does not simulate absorption or scattering effects Installation ============
+You can install from ``pip`` using .. code-block:: sh pip install tof You can
 install from ``conda`` using .. code-block:: sh conda install -c conda-forge -
 c scipp tof .. toctree:: :maxdepth: 2 :hidden: short-example sources components
 multiple-pulses api Release notes
 github.com/scipp/tof/releases>
```

### Comparing `tof-23.5.2/docs/multiple-pulses.ipynb` & `tof-23.5.3/docs/multiple-pulses.ipynb`

 * *Files identical despite different names*

### Comparing `tof-23.5.2/docs/short-example.ipynb` & `tof-23.5.3/docs/short-example.ipynb`

 * *Files identical despite different names*

### Comparing `tof-23.5.2/docs/sources.ipynb` & `tof-23.5.3/docs/sources.ipynb`

 * *Files identical despite different names*

### Comparing `tof-23.5.2/pyproject.toml` & `tof-23.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tof-23.5.2/requirements/ci.txt` & `tof-23.5.3/requirements/ci.txt`

 * *Files identical despite different names*

### Comparing `tof-23.5.2/requirements/docs.txt` & `tof-23.5.3/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `tof-23.5.2/requirements/static.txt` & `tof-23.5.3/requirements/static.txt`

 * *Files identical despite different names*

### Comparing `tof-23.5.2/src/tof/chopper.py` & `tof-23.5.3/src/tof/chopper.py`

 * *Files identical despite different names*

### Comparing `tof-23.5.2/src/tof/component.py` & `tof-23.5.3/src/tof/component.py`

 * *Files identical despite different names*

### Comparing `tof-23.5.2/src/tof/detector.py` & `tof-23.5.3/src/tof/detector.py`

 * *Files identical despite different names*

### Comparing `tof-23.5.2/src/tof/facilities/ess_pulse.py` & `tof-23.5.3/src/tof/facilities/ess_pulse.py`

 * *Files identical despite different names*

### Comparing `tof-23.5.2/src/tof/model.py` & `tof-23.5.3/src/tof/model.py`

 * *Files identical despite different names*

### Comparing `tof-23.5.2/src/tof/result.py` & `tof-23.5.3/src/tof/result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
+from __future__ import annotations
+
 from functools import reduce
 from itertools import chain
 from types import MappingProxyType
 from typing import Dict, Optional, Tuple, Union
 
 import matplotlib.pyplot as plt
 import numpy as np
```

### Comparing `tof-23.5.2/src/tof/source.py` & `tof-23.5.3/src/tof/source.py`

 * *Files identical despite different names*

### Comparing `tof-23.5.2/src/tof/utils.py` & `tof-23.5.3/src/tof/utils.py`

 * *Files identical despite different names*

### Comparing `tof-23.5.2/src/tof.egg-info/PKG-INFO` & `tof-23.5.3/src/tof.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tof
-Version: 23.5.2
+Version: 23.5.3
 Summary: A simple tool to create time-of-flight chopper cascade diagrams
 Author: Neil Vaytet
 License: BSD-3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -14,14 +14,20 @@
 
 [![Documentation Status](https://readthedocs.org/projects/tof/badge/?version=latest)](https://tof.readthedocs.io/en/latest/?badge=latest)
 
 # tof
 
 A simple tool to create time-of-flight chopper cascade diagrams
 
+**Scope:**
+
+- ``tof`` is designed to be simple and lightweight, it will never replace [McStas](https://www.mcstas.org/)
+- it assumes all neutrons travel in a straight line
+- it does not simulate absorption or scattering effects
+
 ## Installation
 
 ```sh
 pip install tof
 ```
 
 ## Documentation
```

### Comparing `tof-23.5.2/src/tof.egg-info/SOURCES.txt` & `tof-23.5.3/src/tof.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tof-23.5.2/tests/chopper_test.py` & `tof-23.5.3/tests/chopper_test.py`

 * *Files identical despite different names*

### Comparing `tof-23.5.2/tests/common.py` & `tof-23.5.3/tests/common.py`

 * *Files identical despite different names*

### Comparing `tof-23.5.2/tests/model_test.py` & `tof-23.5.3/tests/model_test.py`

 * *Files identical despite different names*

### Comparing `tof-23.5.2/tests/result_test.py` & `tof-23.5.3/tests/result_test.py`

 * *Files identical despite different names*

### Comparing `tof-23.5.2/tests/source_test.py` & `tof-23.5.3/tests/source_test.py`

 * *Files identical despite different names*

### Comparing `tof-23.5.2/tox.ini` & `tof-23.5.3/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tox]
-envlist = py310
+envlist = py38
 isolated_build = true
 
 [testenv]
 deps = -r requirements/test.txt
 commands = pytest
 
 [testenv:docs]
 description = invoke sphinx-build to build the HTML docs
-basepython = python3.10
+basepython = python3.8
 deps = {posargs:}
        -r requirements/docs.txt
 allowlist_externals=find
 commands = python -m sphinx -j2 -v -b html -d {toxworkdir}/docs_doctrees docs html
            find html -type f -name "*.ipynb" -not -path "html/_sources/*" -delete
 
 [testenv:static]
 description = Code formatting and static analysis
-basepython = python3.10
+basepython = python3.8
 skip_install = true
 deps = -r requirements/static.txt
 allowlist_externals = sh
 # The first run of pre-commit may reformat files. If this happens, it returns 1 but this
 # should not fail the job. So just run again if it fails. A second failure means that
 # either the different formatters can't agree on a format or that static analysis failed.
 commands = sh -c 'pre-commit run -a || (echo "" && pre-commit run -a)'
```

