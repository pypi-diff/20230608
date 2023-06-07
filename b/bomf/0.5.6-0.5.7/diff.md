# Comparing `tmp/bomf-0.5.6.tar.gz` & `tmp/bomf-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bomf-0.5.6.tar", last modified: Tue Jun  6 21:44:57 2023, max compression
+gzip compressed data, was "bomf-0.5.7.tar", last modified: Wed Jun  7 22:39:30 2023, max compression
```

## Comparing `bomf-0.5.6.tar` & `bomf-0.5.7.tar`

### file list

```diff
@@ -1,69 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:44:57.079460 bomf-0.5.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:44:57.075460 bomf-0.5.6/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-06 21:44:49.000000 bomf-0.5.6/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:44:57.075460 bomf-0.5.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-06 21:44:49.000000 bomf-0.5.6/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-06-06 21:44:49.000000 bomf-0.5.6/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-06 21:44:49.000000 bomf-0.5.6/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-06 21:44:49.000000 bomf-0.5.6/.github/workflows/no_byte_order_mark.yml
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-06 21:44:49.000000 bomf-0.5.6/.github/workflows/packaging_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-06 21:44:49.000000 bomf-0.5.6/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-06 21:44:49.000000 bomf-0.5.6/.github/workflows/pythonlint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-06 21:44:49.000000 bomf-0.5.6/.github/workflows/unittests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-06 21:44:49.000000 bomf-0.5.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-06 21:44:49.000000 bomf-0.5.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-06 21:44:49.000000 bomf-0.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-06-06 21:44:57.079460 bomf-0.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-06-06 21:44:49.000000 bomf-0.5.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-06 21:44:49.000000 bomf-0.5.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-06 21:44:49.000000 bomf-0.5.6/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-06 21:44:49.000000 bomf-0.5.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-06 21:44:57.079460 bomf-0.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-06 21:44:49.000000 bomf-0.5.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:44:57.071459 bomf-0.5.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:44:57.075460 bomf-0.5.6/src/bomf/
--rw-r--r--   0 runner    (1001) docker     (123)     7846 2023-06-06 21:44:49.000000 bomf-0.5.6/src/bomf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:44:57.075460 bomf-0.5.6/src/bomf/filter/
--rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-06-06 21:44:49.000000 bomf-0.5.6/src/bomf/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-06-06 21:44:49.000000 bomf-0.5.6/src/bomf/filter/sourcedataproviderfilter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:44:57.075460 bomf-0.5.6/src/bomf/loader/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-06 21:44:49.000000 bomf-0.5.6/src/bomf/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-06-06 21:44:49.000000 bomf-0.5.6/src/bomf/loader/entityloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:44:57.075460 bomf-0.5.6/src/bomf/mapper/
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-06-06 21:44:49.000000 bomf-0.5.6/src/bomf/mapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:44:57.075460 bomf-0.5.6/src/bomf/model/
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-06-06 21:44:49.000000 bomf-0.5.6/src/bomf/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:44:57.075460 bomf-0.5.6/src/bomf/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-06-06 21:44:49.000000 bomf-0.5.6/src/bomf/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-06 21:44:49.000000 bomf-0.5.6/src/bomf/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:44:57.075460 bomf-0.5.6/src/bomf/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-06 21:44:49.000000 bomf-0.5.6/src/bomf/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:44:57.079460 bomf-0.5.6/src/bomf/validation/core/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-06 21:44:49.000000 bomf-0.5.6/src/bomf/validation/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-06-06 21:44:49.000000 bomf-0.5.6/src/bomf/validation/core/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     7672 2023-06-06 21:44:49.000000 bomf-0.5.6/src/bomf/validation/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    17577 2023-06-06 21:44:49.000000 bomf-0.5.6/src/bomf/validation/core/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-06 21:44:49.000000 bomf-0.5.6/src/bomf/validation/core/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-06 21:44:49.000000 bomf-0.5.6/src/bomf/validation/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-06-06 21:44:49.000000 bomf-0.5.6/src/bomf/validation/core/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-06-06 21:44:49.000000 bomf-0.5.6/src/bomf/validation/path_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-06-06 21:44:49.000000 bomf-0.5.6/src/bomf/validation/query_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-06 21:44:49.000000 bomf-0.5.6/src/bomf/validation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:44:57.075460 bomf-0.5.6/src/bomf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-06-06 21:44:56.000000 bomf-0.5.6/src/bomf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-06 21:44:56.000000 bomf-0.5.6/src/bomf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 21:44:56.000000 bomf-0.5.6/src/bomf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 21:44:56.000000 bomf-0.5.6/src/bomf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-06 21:44:56.000000 bomf-0.5.6/src/bomf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-06 21:44:56.000000 bomf-0.5.6/src/bomf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-06 21:44:49.000000 bomf-0.5.6/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:44:57.079460 bomf-0.5.6/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-06 21:44:49.000000 bomf-0.5.6/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-06 21:44:49.000000 bomf-0.5.6/unittests/example_source_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-06 21:44:49.000000 bomf-0.5.6/unittests/test_bo4e_data_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-06-06 21:44:49.000000 bomf-0.5.6/unittests/test_entity_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-06-06 21:44:49.000000 bomf-0.5.6/unittests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-06-06 21:44:49.000000 bomf-0.5.6/unittests/test_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-06-06 21:44:49.000000 bomf-0.5.6/unittests/test_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-06-06 21:44:49.000000 bomf-0.5.6/unittests/test_source_data_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    21291 2023-06-06 21:44:49.000000 bomf-0.5.6/unittests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:39:30.668971 bomf-0.5.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:39:30.664971 bomf-0.5.7/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-07 22:39:23.000000 bomf-0.5.7/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:39:30.664971 bomf-0.5.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-07 22:39:23.000000 bomf-0.5.7/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-06-07 22:39:23.000000 bomf-0.5.7/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-07 22:39:23.000000 bomf-0.5.7/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-07 22:39:23.000000 bomf-0.5.7/.github/workflows/no_byte_order_mark.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-07 22:39:23.000000 bomf-0.5.7/.github/workflows/packaging_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-07 22:39:23.000000 bomf-0.5.7/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-07 22:39:23.000000 bomf-0.5.7/.github/workflows/pythonlint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-07 22:39:23.000000 bomf-0.5.7/.github/workflows/unittests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-07 22:39:23.000000 bomf-0.5.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-07 22:39:23.000000 bomf-0.5.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-07 22:39:23.000000 bomf-0.5.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-06-07 22:39:30.668971 bomf-0.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-06-07 22:39:23.000000 bomf-0.5.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-07 22:39:23.000000 bomf-0.5.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-07 22:39:23.000000 bomf-0.5.7/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-07 22:39:23.000000 bomf-0.5.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-07 22:39:30.668971 bomf-0.5.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-07 22:39:23.000000 bomf-0.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:39:30.660971 bomf-0.5.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:39:30.664971 bomf-0.5.7/src/bomf/
+-rw-r--r--   0 runner    (1001) docker     (123)     7846 2023-06-07 22:39:23.000000 bomf-0.5.7/src/bomf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:39:30.664971 bomf-0.5.7/src/bomf/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-06-07 22:39:23.000000 bomf-0.5.7/src/bomf/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-06-07 22:39:23.000000 bomf-0.5.7/src/bomf/filter/sourcedataproviderfilter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:39:30.664971 bomf-0.5.7/src/bomf/loader/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-07 22:39:23.000000 bomf-0.5.7/src/bomf/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-06-07 22:39:23.000000 bomf-0.5.7/src/bomf/loader/entityloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:39:30.664971 bomf-0.5.7/src/bomf/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-06-07 22:39:23.000000 bomf-0.5.7/src/bomf/mapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:39:30.664971 bomf-0.5.7/src/bomf/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-06-07 22:39:23.000000 bomf-0.5.7/src/bomf/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:39:30.664971 bomf-0.5.7/src/bomf/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-06-07 22:39:23.000000 bomf-0.5.7/src/bomf/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-07 22:39:23.000000 bomf-0.5.7/src/bomf/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:39:30.664971 bomf-0.5.7/src/bomf/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-07 22:39:23.000000 bomf-0.5.7/src/bomf/validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:39:30.664971 bomf-0.5.7/src/bomf/validation/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-07 22:39:23.000000 bomf-0.5.7/src/bomf/validation/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-06-07 22:39:23.000000 bomf-0.5.7/src/bomf/validation/core/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7672 2023-06-07 22:39:23.000000 bomf-0.5.7/src/bomf/validation/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17577 2023-06-07 22:39:23.000000 bomf-0.5.7/src/bomf/validation/core/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-07 22:39:23.000000 bomf-0.5.7/src/bomf/validation/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-07 22:39:23.000000 bomf-0.5.7/src/bomf/validation/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-06-07 22:39:23.000000 bomf-0.5.7/src/bomf/validation/core/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-06-07 22:39:23.000000 bomf-0.5.7/src/bomf/validation/path_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-06-07 22:39:23.000000 bomf-0.5.7/src/bomf/validation/query_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-07 22:39:23.000000 bomf-0.5.7/src/bomf/validation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:39:30.664971 bomf-0.5.7/src/bomf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-06-07 22:39:30.000000 bomf-0.5.7/src/bomf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-07 22:39:30.000000 bomf-0.5.7/src/bomf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 22:39:30.000000 bomf-0.5.7/src/bomf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 22:39:30.000000 bomf-0.5.7/src/bomf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-07 22:39:30.000000 bomf-0.5.7/src/bomf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-07 22:39:30.000000 bomf-0.5.7/src/bomf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-07 22:39:23.000000 bomf-0.5.7/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:39:30.668971 bomf-0.5.7/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-07 22:39:23.000000 bomf-0.5.7/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-07 22:39:23.000000 bomf-0.5.7/unittests/example_source_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-07 22:39:23.000000 bomf-0.5.7/unittests/test_bo4e_data_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-06-07 22:39:23.000000 bomf-0.5.7/unittests/test_entity_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-06-07 22:39:23.000000 bomf-0.5.7/unittests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-07 22:39:23.000000 bomf-0.5.7/unittests/test_list_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-06-07 22:39:23.000000 bomf-0.5.7/unittests/test_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-06-07 22:39:23.000000 bomf-0.5.7/unittests/test_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-06-07 22:39:23.000000 bomf-0.5.7/unittests/test_source_data_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21291 2023-06-07 22:39:23.000000 bomf-0.5.7/unittests/test_validation.py
```

### Comparing `bomf-0.5.6/.github/dependabot.yml` & `bomf-0.5.7/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.6/.github/workflows/black.yml` & `bomf-0.5.7/.github/workflows/black.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.6/.github/workflows/codeql-analysis.yml` & `bomf-0.5.7/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.6/.github/workflows/coverage.yml` & `bomf-0.5.7/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.6/.github/workflows/packaging_test.yml` & `bomf-0.5.7/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.6/.github/workflows/python-publish.yml` & `bomf-0.5.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.6/.github/workflows/pythonlint.yml` & `bomf-0.5.7/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.6/.github/workflows/unittests.yml` & `bomf-0.5.7/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.6/.gitignore` & `bomf-0.5.7/.gitignore`

 * *Files identical despite different names*

### Comparing `bomf-0.5.6/.pre-commit-config.yaml` & `bomf-0.5.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.6/LICENSE` & `bomf-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bomf-0.5.6/PKG-INFO` & `bomf-0.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bomf
-Version: 0.5.6
+Version: 0.5.7
 Summary: BO4E Migration Framework
 Home-page: https://github.com/Hochfrequenz/bo4e_migration_framework
 Author: Hochfrequenz Unternehmensberatung GmbH
 Author-email: info@hochfrequenz.de
 License: mit
 Project-URL: Documentation, https://github.com/Hochfrequenz/bo4e_migration_framework
 Project-URL: Code, https://github.com/Hochfrequenz/bo4e_migration_framework
```

### Comparing `bomf-0.5.6/README.md` & `bomf-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `bomf-0.5.6/pyproject.toml` & `bomf-0.5.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.6/requirements.txt` & `bomf-0.5.7/requirements.txt`

 * *Files identical despite different names*

### Comparing `bomf-0.5.6/setup.cfg` & `bomf-0.5.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `bomf-0.5.6/src/bomf/__init__.py` & `bomf-0.5.7/src/bomf/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.6/src/bomf/filter/__init__.py` & `bomf-0.5.7/src/bomf/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.6/src/bomf/filter/sourcedataproviderfilter.py` & `bomf-0.5.7/src/bomf/filter/sourcedataproviderfilter.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.6/src/bomf/loader/entityloader.py` & `bomf-0.5.7/src/bomf/loader/entityloader.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.6/src/bomf/model/__init__.py` & `bomf-0.5.7/src/bomf/model/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.6/src/bomf/provider/__init__.py` & `bomf-0.5.7/src/bomf/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.6/src/bomf/validation/core/analysis.py` & `bomf-0.5.7/src/bomf/validation/core/analysis.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.6/src/bomf/validation/core/errors.py` & `bomf-0.5.7/src/bomf/validation/core/errors.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.6/src/bomf/validation/core/execution.py` & `bomf-0.5.7/src/bomf/validation/core/execution.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.6/src/bomf/validation/core/types.py` & `bomf-0.5.7/src/bomf/validation/core/types.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.6/src/bomf/validation/core/utils.py` & `bomf-0.5.7/src/bomf/validation/core/utils.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.6/src/bomf/validation/core/validator.py` & `bomf-0.5.7/src/bomf/validation/core/validator.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.6/src/bomf/validation/path_map.py` & `bomf-0.5.7/src/bomf/validation/path_map.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.6/src/bomf/validation/query_map.py` & `bomf-0.5.7/src/bomf/validation/query_map.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.6/src/bomf/validation/utils.py` & `bomf-0.5.7/src/bomf/validation/utils.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.6/src/bomf.egg-info/PKG-INFO` & `bomf-0.5.7/src/bomf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bomf
-Version: 0.5.6
+Version: 0.5.7
 Summary: BO4E Migration Framework
 Home-page: https://github.com/Hochfrequenz/bo4e_migration_framework
 Author: Hochfrequenz Unternehmensberatung GmbH
 Author-email: info@hochfrequenz.de
 License: mit
 Project-URL: Documentation, https://github.com/Hochfrequenz/bo4e_migration_framework
 Project-URL: Code, https://github.com/Hochfrequenz/bo4e_migration_framework
```

### Comparing `bomf-0.5.6/src/bomf.egg-info/SOURCES.txt` & `bomf-0.5.7/src/bomf.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -44,11 +44,12 @@
 src/bomf/validation/core/utils.py
 src/bomf/validation/core/validator.py
 unittests/__init__.py
 unittests/example_source_data.json
 unittests/test_bo4e_data_set.py
 unittests/test_entity_loader.py
 unittests/test_filter.py
+unittests/test_list_conversion.py
 unittests/test_mapper.py
 unittests/test_migration.py
 unittests/test_source_data_provider.py
 unittests/test_validation.py
```

### Comparing `bomf-0.5.6/tox.ini` & `bomf-0.5.7/tox.ini`

 * *Files identical despite different names*

### Comparing `bomf-0.5.6/unittests/test_bo4e_data_set.py` & `bomf-0.5.7/unittests/test_bo4e_data_set.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.6/unittests/test_entity_loader.py` & `bomf-0.5.7/unittests/test_entity_loader.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.6/unittests/test_filter.py` & `bomf-0.5.7/unittests/test_filter.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.6/unittests/test_mapper.py` & `bomf-0.5.7/unittests/test_mapper.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.6/unittests/test_migration.py` & `bomf-0.5.7/unittests/test_migration.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 Tests the overall data flow using bomf.
 """
 from typing import Optional
 from unittest.mock import Mock
 
 from injector import Binder, Injector
 
-from injector import Binder, Injector
-
 from bomf import (
     Bo4eDataSetToTargetMapper,
     EntityLoader,
     Filter,
     IntermediateDataSet,
     MigrationStrategy,
     SourceDataProvider,
```

### Comparing `bomf-0.5.6/unittests/test_source_data_provider.py` & `bomf-0.5.7/unittests/test_source_data_provider.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.6/unittests/test_validation.py` & `bomf-0.5.7/unittests/test_validation.py`

 * *Files identical despite different names*

