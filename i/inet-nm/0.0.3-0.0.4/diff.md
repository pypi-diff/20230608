# Comparing `tmp/inet-nm-0.0.3.tar.gz` & `tmp/inet-nm-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inet-nm-0.0.3.tar", last modified: Wed Jun  7 11:21:48 2023, max compression
+gzip compressed data, was "inet-nm-0.0.4.tar", last modified: Thu Jun  8 11:47:24 2023, max compression
```

## Comparing `inet-nm-0.0.3.tar` & `inet-nm-0.0.4.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:21:48.012292 inet-nm-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-07 11:21:04.000000 inet-nm-0.0.3/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:21:47.984292 inet-nm-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:21:47.996292 inet-nm-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-07 11:21:04.000000 inet-nm-0.0.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-07 11:21:04.000000 inet-nm-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-07 11:21:04.000000 inet-nm-0.0.3/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-07 11:21:04.000000 inet-nm-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-07 11:21:04.000000 inet-nm-0.0.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-07 11:21:04.000000 inet-nm-0.0.3/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-07 11:21:04.000000 inet-nm-0.0.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    10522 2023-06-07 11:21:04.000000 inet-nm-0.0.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-07 11:21:04.000000 inet-nm-0.0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9437 2023-06-07 11:21:48.012292 inet-nm-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-06-07 11:21:04.000000 inet-nm-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:21:48.000292 inet-nm-0.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-07 11:21:04.000000 inet-nm-0.0.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:21:48.000292 inet-nm-0.0.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-07 11:21:04.000000 inet-nm-0.0.3/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-07 11:21:04.000000 inet-nm-0.0.3/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-07 11:21:04.000000 inet-nm-0.0.3/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10022 2023-06-07 11:21:04.000000 inet-nm-0.0.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-07 11:21:04.000000 inet-nm-0.0.3/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-07 11:21:04.000000 inet-nm-0.0.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-07 11:21:04.000000 inet-nm-0.0.3/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-07 11:21:04.000000 inet-nm-0.0.3/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-07 11:21:04.000000 inet-nm-0.0.3/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-07 11:21:04.000000 inet-nm-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-07 11:21:04.000000 inet-nm-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-07 11:21:48.016292 inet-nm-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-07 11:21:04.000000 inet-nm-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:21:47.988292 inet-nm-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:21:48.004292 inet-nm-0.0.3/src/inet_nm/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-07 11:21:04.000000 inet-nm-0.0.3/src/inet_nm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-06-07 11:21:04.000000 inet-nm-0.0.3/src/inet_nm/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9309 2023-06-07 11:21:04.000000 inet-nm-0.0.3/src/inet_nm/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     7017 2023-06-07 11:21:04.000000 inet-nm-0.0.3/src/inet_nm/commissioner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-06-07 11:21:04.000000 inet-nm-0.0.3/src/inet_nm/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-06-07 11:21:04.000000 inet-nm-0.0.3/src/inet_nm/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-06-07 11:21:04.000000 inet-nm-0.0.3/src/inet_nm/filelock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-07 11:21:04.000000 inet-nm-0.0.3/src/inet_nm/locking.py
--rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-06-07 11:21:04.000000 inet-nm-0.0.3/src/inet_nm/runner_apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-06-07 11:21:04.000000 inet-nm-0.0.3/src/inet_nm/runner_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-07 11:21:04.000000 inet-nm-0.0.3/src/inet_nm/runner_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-07 11:21:04.000000 inet-nm-0.0.3/src/inet_nm/update_os_board_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:21:48.008293 inet-nm-0.0.3/src/inet_nm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9437 2023-06-07 11:21:47.000000 inet-nm-0.0.3/src/inet_nm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-07 11:21:47.000000 inet-nm-0.0.3/src/inet_nm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 11:21:47.000000 inet-nm-0.0.3/src/inet_nm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-07 11:21:47.000000 inet-nm-0.0.3/src/inet_nm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 11:21:47.000000 inet-nm-0.0.3/src/inet_nm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-07 11:21:47.000000 inet-nm-0.0.3/src/inet_nm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-07 11:21:47.000000 inet-nm-0.0.3/src/inet_nm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:21:48.012292 inet-nm-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-07 11:21:04.000000 inet-nm-0.0.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-06-07 11:21:04.000000 inet-nm-0.0.3/tests/test_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-07 11:21:04.000000 inet-nm-0.0.3/tests/test_comissioner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-07 11:21:04.000000 inet-nm-0.0.3/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-07 11:21:04.000000 inet-nm-0.0.3/tests/test_data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-07 11:21:04.000000 inet-nm-0.0.3/tests/test_filelock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-06-07 11:21:04.000000 inet-nm-0.0.3/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-06-07 11:21:04.000000 inet-nm-0.0.3/tests/test_locking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-07 11:21:04.000000 inet-nm-0.0.3/tests/test_runner_apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-07 11:21:04.000000 inet-nm-0.0.3/tests/test_runner_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-06-07 11:21:04.000000 inet-nm-0.0.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:47:24.088981 inet-nm-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-08 11:46:43.000000 inet-nm-0.0.4/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:47:24.080981 inet-nm-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:47:24.084981 inet-nm-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-08 11:46:43.000000 inet-nm-0.0.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-08 11:46:43.000000 inet-nm-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-08 11:46:43.000000 inet-nm-0.0.4/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-08 11:46:43.000000 inet-nm-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-08 11:46:43.000000 inet-nm-0.0.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-08 11:46:43.000000 inet-nm-0.0.4/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-08 11:46:43.000000 inet-nm-0.0.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10522 2023-06-08 11:46:43.000000 inet-nm-0.0.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-08 11:46:43.000000 inet-nm-0.0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-06-08 11:47:24.088981 inet-nm-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-06-08 11:46:43.000000 inet-nm-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:47:24.084981 inet-nm-0.0.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-08 11:46:43.000000 inet-nm-0.0.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:47:24.084981 inet-nm-0.0.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-08 11:46:43.000000 inet-nm-0.0.4/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-08 11:46:43.000000 inet-nm-0.0.4/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-08 11:46:43.000000 inet-nm-0.0.4/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10022 2023-06-08 11:46:43.000000 inet-nm-0.0.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-08 11:46:43.000000 inet-nm-0.0.4/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-08 11:46:43.000000 inet-nm-0.0.4/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-08 11:46:43.000000 inet-nm-0.0.4/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-08 11:46:43.000000 inet-nm-0.0.4/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-08 11:46:43.000000 inet-nm-0.0.4/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-08 11:46:43.000000 inet-nm-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-08 11:46:43.000000 inet-nm-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-08 11:47:24.088981 inet-nm-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-08 11:46:43.000000 inet-nm-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:47:24.080981 inet-nm-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:47:24.084981 inet-nm-0.0.4/src/inet_nm/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-08 11:46:43.000000 inet-nm-0.0.4/src/inet_nm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-06-08 11:46:43.000000 inet-nm-0.0.4/src/inet_nm/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9309 2023-06-08 11:46:43.000000 inet-nm-0.0.4/src/inet_nm/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7683 2023-06-08 11:46:43.000000 inet-nm-0.0.4/src/inet_nm/commissioner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-06-08 11:46:43.000000 inet-nm-0.0.4/src/inet_nm/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-06-08 11:46:43.000000 inet-nm-0.0.4/src/inet_nm/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-06-08 11:46:43.000000 inet-nm-0.0.4/src/inet_nm/filelock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-08 11:46:43.000000 inet-nm-0.0.4/src/inet_nm/locking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-06-08 11:46:43.000000 inet-nm-0.0.4/src/inet_nm/runner_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-06-08 11:46:43.000000 inet-nm-0.0.4/src/inet_nm/runner_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-06-08 11:46:43.000000 inet-nm-0.0.4/src/inet_nm/runner_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-08 11:46:43.000000 inet-nm-0.0.4/src/inet_nm/update_os_board_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:47:24.084981 inet-nm-0.0.4/src/inet_nm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-06-08 11:47:24.000000 inet-nm-0.0.4/src/inet_nm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-08 11:47:24.000000 inet-nm-0.0.4/src/inet_nm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 11:47:24.000000 inet-nm-0.0.4/src/inet_nm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-08 11:47:24.000000 inet-nm-0.0.4/src/inet_nm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 11:47:23.000000 inet-nm-0.0.4/src/inet_nm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-08 11:47:24.000000 inet-nm-0.0.4/src/inet_nm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-08 11:47:24.000000 inet-nm-0.0.4/src/inet_nm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:47:24.088981 inet-nm-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-08 11:46:43.000000 inet-nm-0.0.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-06-08 11:46:43.000000 inet-nm-0.0.4/tests/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-08 11:46:43.000000 inet-nm-0.0.4/tests/test_comissioner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-08 11:46:43.000000 inet-nm-0.0.4/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-08 11:46:43.000000 inet-nm-0.0.4/tests/test_data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-08 11:46:43.000000 inet-nm-0.0.4/tests/test_filelock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-06-08 11:46:43.000000 inet-nm-0.0.4/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-06-08 11:46:43.000000 inet-nm-0.0.4/tests/test_locking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-08 11:46:43.000000 inet-nm-0.0.4/tests/test_runner_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-08 11:46:43.000000 inet-nm-0.0.4/tests/test_runner_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-06-08 11:46:43.000000 inet-nm-0.0.4/tox.ini
```

### Comparing `inet-nm-0.0.3/.coveragerc` & `inet-nm-0.0.4/.coveragerc`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.3/.github/workflows/ci.yml` & `inet-nm-0.0.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.3/.gitignore` & `inet-nm-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.3/.pre-commit-config.yaml` & `inet-nm-0.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.3/.readthedocs.yml` & `inet-nm-0.0.4/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.3/CHANGELOG.md` & `inet-nm-0.0.4/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 # Changelog
 
-## Version 0.0.2 (development)
+## Version 0.0.4 (development)
+ - feat: Add node id output to exec command
+ - fix: cleanup incorrect documentation
+
+## Version 0.0.3 (development)
  - fix: handle empty files and check early
  - fix: handle broken return types of empty files
  - cleanup: remove RIOT from src
  - rework: make config classes
 
 ## Version 0.0.2 (development)
```

### Comparing `inet-nm-0.0.3/CONTRIBUTING.md` & `inet-nm-0.0.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.3/LICENSE.txt` & `inet-nm-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.3/PKG-INFO` & `inet-nm-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inet-nm
-Version: 0.0.3
+Version: 0.0.4
 Summary: cli application for managing nodes
 Home-page: https://github.com/inetrg/inet-nm
 Author: Kevin Weiss
 Author-email: weiss.kevin604@gmail.com
 License: MIT
 Project-URL: Documentation, https://inet-nm.readthedocs.io/en/stable/
 Project-URL: Source, https://github.com/inetrg/inet-nm
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Provides-Extra: testing
 Provides-Extra: all
 License-File: LICENSE.txt
 
-[![CI Tests](https://github.com/inetrg/inet-nm/actions/workflows/ci.yml)](https://github.com/inetrg/inet-nm/actions/workflows/ci.yml/badge.svg)
+[![CI Tests](https://github.com/inetrg/inet-nm/actions/workflows/ci.yml/badge.svg)](https://github.com/inetrg/inet-nm/actions/workflows/ci.yml)
 [![ReadTheDocs](https://readthedocs.org/projects/inet-nm/badge/?version=latest)](https://inet-nm.readthedocs.io/en/stable/)
 [![PyPI-Server](https://img.shields.io/pypi/v/inet-nm.svg)](https://pypi.org/project/inet-nm/)
 [![Monthly Downloads](https://pepy.tech/badge/inet-nm/month)](https://pepy.tech/project/inet-nm)
 
 # inet_nm - INET Node Manager
 
 INET Node Manager (inet_nm) is a comprehensive suite of command-line
@@ -265,20 +265,20 @@
 NM_IDX=1
 
 ```
 
 6. While the terminal is still open, run another script.
 This will not use the boards that have been used for interactive session.
 ```
-$ inet-nm-exec "printenv | grep NM_BOARD"
-NM_BOARD=frdm-kw41z
-NM_BOARD=saml11-xpro
-NM_BOARD=remote-revb
-NM_BOARD=esp32-wroom-32
-NM_BOARD=b-l072z-lrwan1
+$ inet-nm-exec "echo NM_BOARD=\$NM_BOARD"
+NODE:0:BOARD:frdm-kw41z: NM_BOARD=frdm-kw41z
+NODE:1:BOARD:saml11-xpro: NM_BOARD=saml11-xpro
+NODE:2:BOARD:remote-revb: NM_BOARD=remote-revb
+NODE:3:BOARD:esp32-wroom-32: NM_BOARD=esp32-wroom-32
+NODE:4:BOARD:b-l072z-lrwan1: NM_BOARD=b-l072z-lrwan1
 ```
 
 ## License
 
 This project is licensed under the terms of the MIT license. See the LICENSE file.
 
 ---
@@ -293,16 +293,17 @@
     - Turn all ports on by default whenever checking connection
     - Turn all unused off commissioned nodes by default once the action is complete
     - flags to prevent power options
     - Generic command to turn on all ports or specific nodes
     - Caching usb locations
 - check if tmux is installed
 - cleanup exception handling
-- Commission fake boards
 - remove all or one board
 - commission ignored devices
 - shell script prepend a string to stdio
 - test paned windows with many many boards
 - allow user boards that will not get overwritten
 - Nice readme with some gifs of usage
 - Add a CLI way and example get the port live based off UID to handle reconnecting within tmux session
 - Improve getting started
+- exec command should exit all threads safely on keyboard interrupt
+- Add a session or exec timeout that will abort if the call takes too long
```

### Comparing `inet-nm-0.0.3/README.md` & `inet-nm-0.0.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![CI Tests](https://github.com/inetrg/inet-nm/actions/workflows/ci.yml)](https://github.com/inetrg/inet-nm/actions/workflows/ci.yml/badge.svg)
+[![CI Tests](https://github.com/inetrg/inet-nm/actions/workflows/ci.yml/badge.svg)](https://github.com/inetrg/inet-nm/actions/workflows/ci.yml)
 [![ReadTheDocs](https://readthedocs.org/projects/inet-nm/badge/?version=latest)](https://inet-nm.readthedocs.io/en/stable/)
 [![PyPI-Server](https://img.shields.io/pypi/v/inet-nm.svg)](https://pypi.org/project/inet-nm/)
 [![Monthly Downloads](https://pepy.tech/badge/inet-nm/month)](https://pepy.tech/project/inet-nm)
 
 # inet_nm - INET Node Manager
 
 INET Node Manager (inet_nm) is a comprehensive suite of command-line
@@ -243,20 +243,20 @@
 NM_IDX=1
 
 ```
 
 6. While the terminal is still open, run another script.
 This will not use the boards that have been used for interactive session.
 ```
-$ inet-nm-exec "printenv | grep NM_BOARD"
-NM_BOARD=frdm-kw41z
-NM_BOARD=saml11-xpro
-NM_BOARD=remote-revb
-NM_BOARD=esp32-wroom-32
-NM_BOARD=b-l072z-lrwan1
+$ inet-nm-exec "echo NM_BOARD=\$NM_BOARD"
+NODE:0:BOARD:frdm-kw41z: NM_BOARD=frdm-kw41z
+NODE:1:BOARD:saml11-xpro: NM_BOARD=saml11-xpro
+NODE:2:BOARD:remote-revb: NM_BOARD=remote-revb
+NODE:3:BOARD:esp32-wroom-32: NM_BOARD=esp32-wroom-32
+NODE:4:BOARD:b-l072z-lrwan1: NM_BOARD=b-l072z-lrwan1
 ```
 
 ## License
 
 This project is licensed under the terms of the MIT license. See the LICENSE file.
 
 ---
@@ -271,16 +271,17 @@
     - Turn all ports on by default whenever checking connection
     - Turn all unused off commissioned nodes by default once the action is complete
     - flags to prevent power options
     - Generic command to turn on all ports or specific nodes
     - Caching usb locations
 - check if tmux is installed
 - cleanup exception handling
-- Commission fake boards
 - remove all or one board
 - commission ignored devices
 - shell script prepend a string to stdio
 - test paned windows with many many boards
 - allow user boards that will not get overwritten
 - Nice readme with some gifs of usage
 - Add a CLI way and example get the port live based off UID to handle reconnecting within tmux session
 - Improve getting started
+- exec command should exit all threads safely on keyboard interrupt
+- Add a session or exec timeout that will abort if the call takes too long
```

### Comparing `inet-nm-0.0.3/docs/Makefile` & `inet-nm-0.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.3/docs/conf.py` & `inet-nm-0.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.3/docs/index.md` & `inet-nm-0.0.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.3/setup.cfg` & `inet-nm-0.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.3/setup.py` & `inet-nm-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.3/src/inet_nm/_helpers.py` & `inet-nm-0.0.4/src/inet_nm/_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -163,28 +163,41 @@
     Interactive user prompt with auto-completion.
 
     Args:
         prompt: Message to display to the user.
         options: List of auto-completion options.
 
     Returns:
-        str: User input.
+        User input.
     """
     if options is None:
         options = []
     completer = _Completer(list(set(options)))
     readline.set_completer_delims(" \t\n;")
     readline.set_completer(completer.complete)
     readline.parse_and_bind("tab: complete")
     readline.set_completion_display_matches_hook(completer.display_matches)
 
     nm_print(prompt)
     return nm_input("> ")
 
 
+def nm_prompt_default_input(prompt: str, default: str) -> str:
+    """
+    Interactive user prompt with auto-completion and default value.
+
+    Args:
+        prompt: Message to display to the user.
+        default: Default value.
+
+        Returns:
+            User input."""
+    return nm_input(f"{prompt} [{default}]: ") or default
+
+
 def nm_prompt_confirm(msg: str, default: bool = False) -> bool:
     """
     Interactive user prompt for confirmation.
 
     Args:
         msg: Message to display to the user.
         default: Default value.
```

### Comparing `inet-nm-0.0.3/src/inet_nm/check.py` & `inet-nm-0.0.4/src/inet_nm/check.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.3/src/inet_nm/commissioner.py` & `inet-nm-0.0.4/src/inet_nm/commissioner.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """This module commissions USB boards."""
 import argparse
+import random
 import sys
 from typing import List, Optional
 
 import pyudev
 
+import inet_nm._helpers as hlp
 import inet_nm.config as cfg
 from inet_nm._helpers import nm_prompt_choice, nm_prompt_confirm, nm_prompt_input
 from inet_nm.data_types import NmNode
 
 
 class TtyNotPresent(Exception):
     """Exception to be raised when a TTY device is not found for a given NmNode."""
@@ -142,34 +144,57 @@
             return board
         if nm_prompt_confirm(
             f"Board {board} not in board list, continue?", default=False
         ):
             return board
 
 
+def mock_device():
+    """Mock a device, useful for boards that do not have USB interfaces"""
+
+    sn = f"{random.randint(0, 10**20)}".zfill(20)
+    sn = hlp.nm_prompt_default_input("Enter serial number", sn)
+    return NmNode(
+        vendor_id="1234",
+        product_id="5678",
+        serial=sn,
+        vendor="generic_vendor",
+        driver="mock",
+        mock=True,
+    )
+
+
 def commission():
     """CLI to commission a USB board."""
     parser = argparse.ArgumentParser(description="Commission USB boards")
     cfg.config_arg(parser)
     parser.add_argument("-b", "--board", help="Name of the board to commission")
     parser.add_argument(
         "-n", "--no-cache", help="Ignore the cache", action="store_true"
     )
+    parser.add_argument(
+        "-m",
+        "--mock-dev",
+        help="Mock a device, useful for boards that do not have USB interfaces",
+        action="store_true",
+    )
 
     args = parser.parse_args()
     nodes_cfg = cfg.NodesConfig(args.config)
     bi_cfg = cfg.BoardInfoConfig(args.config)
     # Check early since we will need to write eventually
     nodes_cfg.check_file(writable=True)
     bi_cfg.check_file(writable=False)
 
     saved_nodes = nodes_cfg.load()
     nm_nodes = (
         get_devices_from_tty() if args.no_cache else get_devices_from_tty(saved_nodes)
     )
+    if args.mock_dev:
+        nm_nodes.append(mock_device())
     print(f"Found {len(saved_nodes)} saved nodes in {args.config}")
 
     try:
         selected_node = select_available_node(nm_nodes)
     except ValueError:
         print("No available nodes found")
         return
```

### Comparing `inet-nm-0.0.3/src/inet_nm/config.py` & `inet-nm-0.0.4/src/inet_nm/config.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.3/src/inet_nm/data_types.py` & `inet-nm-0.0.4/src/inet_nm/data_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,25 +41,27 @@
         product_id: Product ID of the device.
         vendor: Name of the vendor.
         driver: Name of the driver.
         model: Model name of the device.
         uid: Unique ID of the device
         board: Name of the board.
         features_provided: List of features provided by the device.
+        mock: Whether the node is a mock node.
     """
 
     serial: str
     vendor_id: str
     product_id: str
     vendor: str
     driver: str
     model: Optional[str] = None
     uid: Optional[str] = None
     board: Optional[str] = None
     features_provided: Optional[List[str]] = None
+    mock: bool = False
 
     def __post_init__(self):
         """Initialize additional attributes after instantiation."""
         self.features_provided = self.features_provided or []
         self.uid = self.uid or NmNode.calculate_uid(
             self.product_id, self.vendor_id, self.serial
         )
```

### Comparing `inet-nm-0.0.3/src/inet_nm/filelock.py` & `inet-nm-0.0.4/src/inet_nm/filelock.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.3/src/inet_nm/locking.py` & `inet-nm-0.0.4/src/inet_nm/locking.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.3/src/inet_nm/runner_apps.py` & `inet-nm-0.0.4/src/inet_nm/runner_apps.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,40 +8,77 @@
 """
 
 import os
 import subprocess
 import time
 from typing import Dict
 
+from inet_nm._helpers import nm_print
 from inet_nm.data_types import NmNode
 from inet_nm.runner_base import NmNodesRunner
 
 
 class NmShellRunner(NmNodesRunner):
     """Runs shell commands on nodes.
 
     This class inherits from NmNodesRunner and overrides the func method
     to execute shell commands on nodes.
+
+    Attributes:
+        cmd: Command to execute on nodes.
     """
 
     cmd = "echo $NM_IDX"
+    SETUP_WAIT = 0.1
+
+    @staticmethod
+    def _run_command(cmd, prefix, env):
+        process = subprocess.Popen(
+            cmd, env=env, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT
+        )
+        while True:
+            output = process.stdout.readline()
+
+            if output:
+                nm_print(f"{prefix}{output.decode().strip()}")
+            else:
+                # Have a small sleep so we are not burning CPU waiting for output.
+                time.sleep(0.2)
+            poll = process.poll()
+            if poll is not None:
+                break
+        rc = process.returncode
+
+        return rc
 
     def func(self, node: NmNode, idx: int, env: Dict[str, str]):
         """Execute shell commands on nodes.
 
         Args:
             node: Node to run the command on.
             idx: Index of the node.
             env: Environment variables for the command.
         """
+        time.sleep(idx * self.SETUP_WAIT)
         full_env = {**os.environ, **env}  # Merge original and new environment variables
         full_env = {
             k: str(v) for k, v in full_env.items()
         }  # Cast everything in env to a string
-        subprocess.run(self.cmd, shell=True, env=full_env)
+
+        prefix = f"NODE:{idx}"
+        if node.board:
+            prefix += f":BOARD:{node.board}"
+        prefix += ": "
+
+        # Since most use cases are with bash we will use that as the default shell.
+        # This may change as soon as we have a use case that requires a different shell.
+        # Note that the run command exits after one command is executed.
+        # So if we want to loop with a default shell it will exit after the first loop.
+        cmd = f"/bin/bash -c '{self.cmd}'"
+        NmShellRunner._run_command(cmd, prefix=prefix, env=full_env)
 
 
 class NmTmuxBaseRunner(NmNodesRunner):
     """Base class for tmux runners.
 
     This class inherits from NmNodesRunner and sets up a tmux session.
     """
```

### Comparing `inet-nm-0.0.3/src/inet_nm/runner_base.py` & `inet-nm-0.0.4/src/inet_nm/runner_base.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.3/src/inet_nm/runner_cli.py` & `inet-nm-0.0.4/src/inet_nm/runner_cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 
 import inet_nm.check as check
 import inet_nm.config as cfg
 import inet_nm.runner_apps as apps
 
 
 def nm_tmux():
-    parser = argparse.ArgumentParser(description="Commission USB boards")
+    parser = argparse.ArgumentParser(
+        description="Starts interactive sessions for each node."
+    )
     parser.add_argument(
         "-w", "--window", action="store_true", help="Open a window for each node."
     )
     parser.add_argument(
         "-t",
         "--timeout",
         type=float,
@@ -42,17 +44,22 @@
     else:
         with apps.NmTmuxPanedRunner(nodes, default_timeout=timeout) as runner:
             runner.cmd = cmd
             runner.run()
 
 
 def nm_exec():
-    parser = argparse.ArgumentParser(description="Commission USB boards")
+    parser = argparse.ArgumentParser(
+        description="Execute command for each note environment."
+    )
     parser.add_argument(
-        "cmd", type=str, help="Command to send after starting tmux session."
+        "cmd",
+        type=str,
+        help="bash command to execute, ' must be escaped and generally pay"
+        " attention to escape characters.",
     )
     parser.add_argument(
         "-t",
         "--timeout",
         type=float,
         default=None,
         help="Wait until node available in seconds.",
```

### Comparing `inet-nm-0.0.3/src/inet_nm/update_os_board_list.py` & `inet-nm-0.0.4/src/inet_nm/update_os_board_list.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.3/src/inet_nm.egg-info/PKG-INFO` & `inet-nm-0.0.4/src/inet_nm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inet-nm
-Version: 0.0.3
+Version: 0.0.4
 Summary: cli application for managing nodes
 Home-page: https://github.com/inetrg/inet-nm
 Author: Kevin Weiss
 Author-email: weiss.kevin604@gmail.com
 License: MIT
 Project-URL: Documentation, https://inet-nm.readthedocs.io/en/stable/
 Project-URL: Source, https://github.com/inetrg/inet-nm
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Provides-Extra: testing
 Provides-Extra: all
 License-File: LICENSE.txt
 
-[![CI Tests](https://github.com/inetrg/inet-nm/actions/workflows/ci.yml)](https://github.com/inetrg/inet-nm/actions/workflows/ci.yml/badge.svg)
+[![CI Tests](https://github.com/inetrg/inet-nm/actions/workflows/ci.yml/badge.svg)](https://github.com/inetrg/inet-nm/actions/workflows/ci.yml)
 [![ReadTheDocs](https://readthedocs.org/projects/inet-nm/badge/?version=latest)](https://inet-nm.readthedocs.io/en/stable/)
 [![PyPI-Server](https://img.shields.io/pypi/v/inet-nm.svg)](https://pypi.org/project/inet-nm/)
 [![Monthly Downloads](https://pepy.tech/badge/inet-nm/month)](https://pepy.tech/project/inet-nm)
 
 # inet_nm - INET Node Manager
 
 INET Node Manager (inet_nm) is a comprehensive suite of command-line
@@ -265,20 +265,20 @@
 NM_IDX=1
 
 ```
 
 6. While the terminal is still open, run another script.
 This will not use the boards that have been used for interactive session.
 ```
-$ inet-nm-exec "printenv | grep NM_BOARD"
-NM_BOARD=frdm-kw41z
-NM_BOARD=saml11-xpro
-NM_BOARD=remote-revb
-NM_BOARD=esp32-wroom-32
-NM_BOARD=b-l072z-lrwan1
+$ inet-nm-exec "echo NM_BOARD=\$NM_BOARD"
+NODE:0:BOARD:frdm-kw41z: NM_BOARD=frdm-kw41z
+NODE:1:BOARD:saml11-xpro: NM_BOARD=saml11-xpro
+NODE:2:BOARD:remote-revb: NM_BOARD=remote-revb
+NODE:3:BOARD:esp32-wroom-32: NM_BOARD=esp32-wroom-32
+NODE:4:BOARD:b-l072z-lrwan1: NM_BOARD=b-l072z-lrwan1
 ```
 
 ## License
 
 This project is licensed under the terms of the MIT license. See the LICENSE file.
 
 ---
@@ -293,16 +293,17 @@
     - Turn all ports on by default whenever checking connection
     - Turn all unused off commissioned nodes by default once the action is complete
     - flags to prevent power options
     - Generic command to turn on all ports or specific nodes
     - Caching usb locations
 - check if tmux is installed
 - cleanup exception handling
-- Commission fake boards
 - remove all or one board
 - commission ignored devices
 - shell script prepend a string to stdio
 - test paned windows with many many boards
 - allow user boards that will not get overwritten
 - Nice readme with some gifs of usage
 - Add a CLI way and example get the port live based off UID to handle reconnecting within tmux session
 - Improve getting started
+- exec command should exit all threads safely on keyboard interrupt
+- Add a session or exec timeout that will abort if the call takes too long
```

### Comparing `inet-nm-0.0.3/src/inet_nm.egg-info/SOURCES.txt` & `inet-nm-0.0.4/src/inet_nm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.3/tests/test_check.py` & `inet-nm-0.0.4/tests/test_check.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.3/tests/test_comissioner.py` & `inet-nm-0.0.4/tests/test_comissioner.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.3/tests/test_config.py` & `inet-nm-0.0.4/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.3/tests/test_data_types.py` & `inet-nm-0.0.4/tests/test_data_types.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.3/tests/test_filelock.py` & `inet-nm-0.0.4/tests/test_filelock.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.3/tests/test_helpers.py` & `inet-nm-0.0.4/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.3/tests/test_locking.py` & `inet-nm-0.0.4/tests/test_locking.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.3/tests/test_runner_apps.py` & `inet-nm-0.0.4/tests/test_runner_apps.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.3/tests/test_runner_base.py` & `inet-nm-0.0.4/tests/test_runner_base.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.3/tox.ini` & `inet-nm-0.0.4/tox.ini`

 * *Files identical despite different names*

