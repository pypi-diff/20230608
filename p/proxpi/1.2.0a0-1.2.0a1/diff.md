# Comparing `tmp/proxpi-1.2.0a0.tar.gz` & `tmp/proxpi-1.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxpi-1.2.0a0.tar", last modified: Thu May 25 15:02:38 2023, max compression
+gzip compressed data, was "proxpi-1.2.0a1.tar", last modified: Thu Jun  8 09:00:55 2023, max compression
```

## Comparing `proxpi-1.2.0a0.tar` & `proxpi-1.2.0a1.tar`

### file list

```diff
@@ -1,47 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:02:38.560456 proxpi-1.2.0a0/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:02:38.556456 proxpi-1.2.0a0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:02:38.556456 proxpi-1.2.0a0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:02:38.556456 proxpi-1.2.0a0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/.github/workflows/publish-docker-image.yml
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/.github/workflows/publish-python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/.github/workflows/test-python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9521 2023-05-25 15:02:38.560456 proxpi-1.2.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8927 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)    20413 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/app.requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:02:38.556456 proxpi-1.2.0a0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/scripts/benchmark-json-api-response-size.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-25 15:02:38.560456 proxpi-1.2.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:02:38.552456 proxpi-1.2.0a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:02:38.556456 proxpi-1.2.0a0/src/proxpi/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/src/proxpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28628 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/src/proxpi/_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     6953 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/src/proxpi/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:02:38.560456 proxpi-1.2.0a0/src/proxpi/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/src/proxpi/templates/files.html
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/src/proxpi/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/src/proxpi/templates/packages.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:02:38.556456 proxpi-1.2.0a0/src/proxpi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9521 2023-05-25 15:02:38.000000 proxpi-1.2.0a0/src/proxpi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-25 15:02:38.000000 proxpi-1.2.0a0/src/proxpi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 15:02:38.000000 proxpi-1.2.0a0/src/proxpi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-25 15:02:38.000000 proxpi-1.2.0a0/src/proxpi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-25 15:02:38.000000 proxpi-1.2.0a0/src/proxpi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:02:38.560456 proxpi-1.2.0a0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/tests/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18106 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-25 15:02:26.000000 proxpi-1.2.0a0/tests/test_pypi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:00:55.324772 proxpi-1.2.0a1/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:00:55.312772 proxpi-1.2.0a1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:00:55.312772 proxpi-1.2.0a1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:00:55.312772 proxpi-1.2.0a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/.github/workflows/publish-docker-image.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/.github/workflows/publish-python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/.github/workflows/test-python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9521 2023-06-08 09:00:55.324772 proxpi-1.2.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8927 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)    20413 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/app.requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:00:55.316772 proxpi-1.2.0a1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/scripts/benchmark-json-api-response-size.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-08 09:00:55.324772 proxpi-1.2.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:00:55.304772 proxpi-1.2.0a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:00:55.316772 proxpi-1.2.0a1/src/proxpi/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/src/proxpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29418 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/src/proxpi/_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6953 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/src/proxpi/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:00:55.316772 proxpi-1.2.0a1/src/proxpi/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/src/proxpi/templates/files.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/src/proxpi/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/src/proxpi/templates/packages.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:00:55.316772 proxpi-1.2.0a1/src/proxpi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9521 2023-06-08 09:00:55.000000 proxpi-1.2.0a1/src/proxpi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-06-08 09:00:55.000000 proxpi-1.2.0a1/src/proxpi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 09:00:55.000000 proxpi-1.2.0a1/src/proxpi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-08 09:00:55.000000 proxpi-1.2.0a1/src/proxpi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 09:00:55.000000 proxpi-1.2.0a1/src/proxpi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:00:55.320773 proxpi-1.2.0a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/tests/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:00:55.304772 proxpi-1.2.0a1/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:00:55.308772 proxpi-1.2.0a1/tests/data/indexes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:00:55.320773 proxpi-1.2.0a1/tests/data/indexes/extra/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/tests/data/indexes/extra/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/tests/data/indexes/extra/index.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:00:55.320773 proxpi-1.2.0a1/tests/data/indexes/extra/numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/tests/data/indexes/extra/numpy/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/tests/data/indexes/extra/numpy/index.json
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/tests/data/indexes/extra/numpy/numpy-1.23.1-cp310-cp310-macosx_10_9_x86_64.whl
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/tests/data/indexes/extra/numpy/yanked.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:00:55.320773 proxpi-1.2.0a1/tests/data/indexes/extra/scipy/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/tests/data/indexes/extra/scipy/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/tests/data/indexes/extra/scipy/index.json
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/tests/data/indexes/extra/scipy/scipy-1.9.0-cp310-cp310-manylinux_2_17_x86_64.whl
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/tests/data/indexes/extra/scipy/scipy-1.9.0.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/tests/data/indexes/extra/scipy/yanked.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:00:55.324772 proxpi-1.2.0a1/tests/data/indexes/root/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/tests/data/indexes/root/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/tests/data/indexes/root/index.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:00:55.324772 proxpi-1.2.0a1/tests/data/indexes/root/numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/tests/data/indexes/root/numpy/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/tests/data/indexes/root/numpy/index.json
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/tests/data/indexes/root/numpy/numpy-1.23.1-cp310-cp310-manylinux_2_17_x86_64.whl
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/tests/data/indexes/root/numpy/numpy-1.23.1-cp310-cp310-manylinux_2_24_x86_64.whl
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/tests/data/indexes/root/numpy/numpy-1.23.1-cp310-cp310-manylinux_2_24_x86_64.whl.metadata
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/tests/data/indexes/root/numpy/numpy-1.23.1-cp310-cp310-manylinux_2_28_x86_64.whl
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/tests/data/indexes/root/numpy/numpy-1.23.1-cp310-cp310-manylinux_2_28_x86_64.whl.metadata
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/tests/data/indexes/root/numpy/numpy-1.23.1-cp310-cp310-win_amd64.whl
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/tests/data/indexes/root/numpy/numpy-1.23.1.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/tests/data/indexes/root/numpy/yanked.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:00:55.324772 proxpi-1.2.0a1/tests/data/indexes/root/proxpi/
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/tests/data/indexes/root/proxpi/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/tests/data/indexes/root/proxpi/index.json
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/tests/data/indexes/root/proxpi/proxpi-1.0.0-py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/tests/data/indexes/root/proxpi/proxpi-1.0.0.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/tests/data/indexes/root/proxpi/proxpi-1.1.0-py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/tests/data/indexes/root/proxpi/proxpi-1.1.0.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/tests/data/indexes/root/proxpi/yanked.json
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/tests/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1080 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/tests/test-docker-image.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    16472 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-08 09:00:39.000000 proxpi-1.2.0a1/tests/test_pypi.py
```

### Comparing `proxpi-1.2.0a0/.github/ISSUE_TEMPLATE/bug_report.md` & `proxpi-1.2.0a1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `proxpi-1.2.0a0/.github/workflows/publish-python-package.yml` & `proxpi-1.2.0a1/.github/workflows/publish-python-package.yml`

 * *Files 23% similar despite different names*

```diff
@@ -16,12 +16,18 @@
     - name: Install build tools
       run: |
         pip install -U pip
         pip install build
     - name: Build package
       run: |
         pyproject-build --outdir dist/
+    - name: Install package
+      run: pip install dist/*.whl
+    - name: Run unit-tests
+      run: |
+        pip install -r tests/requirements.txt
+        pytest -vvra
     - name: Publish package
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
         user: ${{ secrets.PYPI_USERNAME }}
         password: ${{ secrets.PYPI_PASSWORD }}
```

### Comparing `proxpi-1.2.0a0/.github/workflows/test-python-package.yml` & `proxpi-1.2.0a1/.github/workflows/test-python-package.yml`

 * *Files identical despite different names*

### Comparing `proxpi-1.2.0a0/CODE_OF_CONDUCT.md` & `proxpi-1.2.0a1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `proxpi-1.2.0a0/CONTRIBUTING.md` & `proxpi-1.2.0a1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `proxpi-1.2.0a0/Dockerfile` & `proxpi-1.2.0a1/Dockerfile`

 * *Files identical despite different names*

### Comparing `proxpi-1.2.0a0/LICENSE` & `proxpi-1.2.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `proxpi-1.2.0a0/PKG-INFO` & `proxpi-1.2.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxpi
-Version: 1.2.0a0
+Version: 1.2.0a1
 Summary: PyPI caching mirror
 Home-page: https://github.com/EpicWink/proxpi
 Author: Laurie O
 Author-email: laurie_opperman@hotmail.com
 License: MIT
 Keywords: pypi,index,mirror,cache
 Classifier: Environment :: Console
```

### Comparing `proxpi-1.2.0a0/README.md` & `proxpi-1.2.0a1/README.md`

 * *Files identical despite different names*

### Comparing `proxpi-1.2.0a0/app.requirements.txt` & `proxpi-1.2.0a1/app.requirements.txt`

 * *Files identical despite different names*

### Comparing `proxpi-1.2.0a0/scripts/benchmark-json-api-response-size.py` & `proxpi-1.2.0a1/scripts/benchmark-json-api-response-size.py`

 * *Files identical despite different names*

### Comparing `proxpi-1.2.0a0/setup.cfg` & `proxpi-1.2.0a1/setup.cfg`

 * *Files identical despite different names*

### Comparing `proxpi-1.2.0a0/src/proxpi/_cache.py` & `proxpi-1.2.0a1/src/proxpi/_cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,15 +97,16 @@
 
     def to_json_response(self) -> t.Dict[str, t.Any]:
         """Serialise to JSON response data (with 'url' key)."""
         data = {"filename": self.name, "hashes": self.hashes}
         if self.requires_python is not None:
             data["requires-python"] = self.requires_python
         if self.dist_info_metadata is not None:
-            data["dist-info-metadata"] = self.dist_info_metadata
+            # PEP 714: only emit new key in JSON
+            data["core-metadata"] = self.dist_info_metadata
         if self.gpg_sig is not None:
             data["gpg-sig"] = self.gpg_sig
         if self.yanked is not None:
             data["yanked"] = self.yanked
         return data
 
 
@@ -120,56 +121,66 @@
 
     @classmethod
     def from_html_element(
         cls, el: "lxml.etree.ElementBase", request_url: str
     ) -> "File":
         """Construct from HTML API response."""
         url = urllib.parse.urljoin(request_url, el.attrib["href"])
+
+        attributes = {k: v for k, v in el.attrib.items() if k != "href"}
+
+        # PEP 714: accept both core-metadata attributes, and emit both in HTML
+        if "data-core-metadata" in attributes:
+            attributes["data-dist-info-metadata"] = attributes["data-core-metadata"]
+        elif "data-dist-info-metadata" in attributes:
+            attributes["data-core-metadata"] = attributes["data-dist-info-metadata"]
+
         return cls(
             name=el.text,
             url=url,
             fragment=urllib.parse.urlsplit(url).fragment,
-            attributes={k: v for k, v in el.attrib.items() if k != "href"},
+            attributes=attributes,
         )
 
     @property
     def hashes(self):
         return self._parse_hash(self.fragment)
 
     @property
     def requires_python(self):
         return self.attributes.get("data-requires-python") or None
 
     @property
     def dist_info_metadata(self):
-        metadata = self.attributes.get("data-dist-info-metadata")
+        metadata = self.attributes.get("data-core-metadata")
         if metadata is None:
             return None
         hashes = self._parse_hash(metadata)
         if not hashes:
+            if metadata not in ("", "true"):
+                logger.warning(
+                    f"Invalid metadata attribute value from index: {metadata}"
+                )
             return True  # '': value-less -> true
         return hashes
 
     @property
     def gpg_sig(self):
         has_gpg_sig = self.attributes.get("data-gpg-sig")
         return has_gpg_sig and self.attributes.get("data-gpg-sig") == "true"
 
     @property
     def yanked(self):
         return self.attributes.get("data-yanked") is not None  # '': value-less -> true
 
     @staticmethod
     def _parse_hash(hash_string: str) -> t.Dict[str, str]:
-        try:
-            hash_name, hash_value = hash_string.split("=")
-        except ValueError:
-            if hash_string.count("=") > 0:
-                raise
+        if "=" not in hash_string:
             return {}
+        hash_name, hash_value = hash_string.split("=")
         return {hash_name: hash_value}
 
 
 @dataclasses.dataclass
 class FileFromJSON(File):
     __slots__ = (
         "name",
@@ -193,15 +204,18 @@
     def from_json_response(cls, data: t.Dict[str, t.Any], request_url: str) -> "File":
         """Construct from JSON API response."""
         return cls(
             name=data["filename"],
             url=urllib.parse.urljoin(request_url, data["url"]),
             hashes=data["hashes"],
             requires_python=data.get("requires-python"),
-            dist_info_metadata=data.get("dist-info-metadata"),
+            # PEP 714: accept both core-metadata keys
+            dist_info_metadata=(
+                data.get("core-metadata") or data.get("dist-info-metadata")
+            ),
             gpg_sig=data.get("gpg-sig"),
             yanked=data.get("yanked"),
         )
 
     @property
     def fragment(self) -> str:
         """File URL fragment."""
@@ -213,14 +227,16 @@
         attributes = {}
         if self.requires_python:
             attributes["data-requires-python"] = self.requires_python
         if self.dist_info_metadata:
             attributes["data-dist-info-metadata"] = self._stringify_hashes(
                 self.dist_info_metadata,
             ) if isinstance(self.dist_info_metadata, dict) else ""  # fmt: skip
+            # PEP 714: emit both core-metadata attributes in HTML
+            attributes["data-core-metadata"] = attributes["data-dist-info-metadata"]
         if self.gpg_sig is not None:
             attributes["data-gpg-sig"] = "true" if self.gpg_sig else "false"
         if self.yanked:
             attributes["data-yanked"] = (
                 self.yanked if isinstance(self.yanked, str) else ""
             )
         return attributes
```

### Comparing `proxpi-1.2.0a0/src/proxpi/server.py` & `proxpi-1.2.0a1/src/proxpi/server.py`

 * *Files identical despite different names*

### Comparing `proxpi-1.2.0a0/src/proxpi/templates/index.html` & `proxpi-1.2.0a1/src/proxpi/templates/index.html`

 * *Files identical despite different names*

### Comparing `proxpi-1.2.0a0/src/proxpi.egg-info/PKG-INFO` & `proxpi-1.2.0a1/src/proxpi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxpi
-Version: 1.2.0a0
+Version: 1.2.0a1
 Summary: PyPI caching mirror
 Home-page: https://github.com/EpicWink/proxpi
 Author: Laurie O
 Author-email: laurie_opperman@hotmail.com
 License: MIT
 Keywords: pypi,index,mirror,cache
 Classifier: Environment :: Console
```

### Comparing `proxpi-1.2.0a0/tests/_utils.py` & `proxpi-1.2.0a1/tests/_utils.py`

 * *Files identical despite different names*

### Comparing `proxpi-1.2.0a0/tests/test_integration.py` & `proxpi-1.2.0a1/tests/test_integration.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,29 @@
 """Test ``proxpi`` server."""
 
-import io
 import os
 import hashlib
 import logging
-import tarfile
+import pathlib
 import warnings
 import posixpath
 import contextlib
 import typing as t
 from urllib import parse as urllib_parse
 from unittest import mock
 
 import flask
-import jinja2
 import pytest
 import requests
-import proxpi._cache  # noqa
 import proxpi.server
 import packaging.specifiers
 
 from . import _utils
 
 proxpi_server = proxpi.server
-# noinspection PyProtectedMember
-File = proxpi._cache.FileFromHTML
 
 logging.root.setLevel(logging.DEBUG)
 logging.getLogger("urllib3.connectionpool").setLevel(logging.INFO)
 
 mock_index_response_is_json = False
 
 
@@ -40,171 +35,78 @@
     mock_index_response_is_json = value
     try:
         yield
     finally:
         mock_index_response_is_json = original_mock_index_response_is_json
 
 
-def make_mock_index_app(projects: t.Dict[str, t.List[File]]) -> flask.Flask:
+def make_mock_index_app(index_name: str) -> flask.Flask:
     """Construct a mock package index app.
 
-    Warning: uses ``proxpi``'s templates for index responses, and files are
-    simple
-
     Args:
-        projects: index projects with their files
+        index_name: index name in test data indexes directory
 
     Returns:
         WSGI app for Python package simple repository index
     """
 
-    files_content = {}
-    for project_name_, files_ in projects.items():
-        for file_ in files_:
-            stream = io.BytesIO()
-            with tarfile.TarFile.open(mode="w:gz", fileobj=stream) as tf:
-                tf.addfile(
-                    tarinfo=tarfile.TarInfo(name="spam"),
-                    fileobj=io.BytesIO(file_.url.encode(encoding="utf-8")),
-                )
-            file_content_ = stream.getvalue()
-            files_content[project_name_, file_.name] = file_content_
-            if file_.fragment:
-                assert file_.fragment == "sha256="
-                file_.fragment += hashlib.sha256(file_content_).hexdigest()
-
     app = flask.Flask("proxpi-tests", root_path=os.path.split(__file__)[0])
-    app.jinja_loader = jinja2.PackageLoader("proxpi")
-
-    def build_json_v1_response(data: dict) -> flask.Response:
-        response = flask.jsonify(data)
-        response.mimetype = f"application/vnd.pypi.simple.v1+json"
-        return response
+    indexes_dir_relative_path = pathlib.PurePath("data") / "indexes"
 
     @app.route("/")
-    def list_projects() -> t.Union[str, flask.Response]:
+    def list_projects() -> flask.Response:
         if mock_index_response_is_json:
-            return build_json_v1_response({
-                "meta": {"api-version": "1.0"},
-                "projects": [{"name": n} for n in list(projects)],
-            })  # fmt: skip
-        return flask.render_template("packages.html", package_names=list(projects))
+            file_name = "index.json"
+            mime_type = "application/vnd.pypi.simple.v1+json"
+        else:
+            file_name = "index.html"
+            mime_type = "text/html"
+
+        return flask.send_from_directory(
+            directory=indexes_dir_relative_path,
+            path=pathlib.PurePath(index_name) / file_name,
+            mimetype=mime_type,
+        )
 
     @app.route("/<name>/")
-    def get_project(name: str) -> t.Union[str, flask.Response]:
-        files = projects.get(name)
-        if not files:
-            flask.abort(404)
+    def get_project(name: str) -> flask.Response:
         if mock_index_response_is_json:
-            files_data = []
-            for file in files:
-                file_data = file.to_json_response()
-                file_data["url"] = file.name
-                if (
-                    mock_index_response_is_json == "yanked"
-                    and not file_data.get("yanked")
-                ):
-                    file_data["yanked"] = False
-                files_data.append(file_data)
-            return build_json_v1_response({
-                "meta": {"api-version": "1.0"},
-                "name": name,
-                "files": files_data,
-            })  # fmt: skip
-        return flask.render_template("files.html", package_name=name, files=files)
+            stem = "yanked" if mock_index_response_is_json == "yanked" else "index"
+            file_name = f"{stem}.json"
+            mime_type = "application/vnd.pypi.simple.v1+json"
+        else:
+            file_name = "index.html"
+            mime_type = "text/html"
+
+        return flask.send_from_directory(
+            directory=indexes_dir_relative_path,
+            path=pathlib.PurePath(index_name) / name / file_name,
+            mimetype=mime_type,
+        )
 
     @app.route("/<project_name>/<file_name>")
-    def get_file(project_name: str, file_name: str) -> bytes:
-        file_content = files_content.get((project_name, file_name))
-        if not file_content:
-            flask.abort(404)
-        return file_content
+    def get_file(project_name: str, file_name: str) -> flask.Response:
+        return flask.send_from_directory(
+            directory=indexes_dir_relative_path,
+            path=pathlib.PurePath(index_name) / project_name / file_name,
+            mimetype="application/octect-stream",
+        )
 
     return app
 
 
 @pytest.fixture(scope="module")
 def mock_root_index():
-    app = make_mock_index_app(projects={
-        "proxpi": [
-            File(
-                name="proxpi-1.1.0-py3-none-any.whl",
-                url="spam eggs 42",
-                fragment="sha256=",
-                attributes={"data-requires-python": ">=3.7"},
-            ),
-            File(
-                name="proxpi-1.1.0.tar.gz",
-                url="foo bar 42",
-                fragment="sha256=",
-                attributes={"data-requires-python": ">=3.7"},
-            ),
-            File(
-                name="proxpi-1.0.0-py3-none-any.whl",
-                url="spam eggs 41",
-                fragment="",
-                attributes={},
-            ),
-            File(
-                name="proxpi-1.0.0.tar.gz",
-                url="foo bar 42",
-                fragment="",
-                attributes={"data-requires-python": ""},
-            ),
-        ],
-        "numpy": [
-            File(
-                name="numpy-1.23.1-cp310-cp310-manylinux_2_17_x86_64.whl",
-                url="",
-                fragment="sha256=",
-                attributes={"data-requires-python": ">=3.8"},
-            ),
-            File(
-                name="numpy-1.23.1-cp310-cp310-win_amd64.whl",
-                url="",
-                fragment="sha256=",
-                attributes={"data-requires-python": ">=3.8", "data-yanked": ""},
-            ),
-            File(
-                name="numpy-1.23.1.tar.gz",
-                url="foo bar 42",
-                fragment="sha256=",
-                attributes={"data-requires-python": ">=3.8"},
-            ),
-        ],
-    })  # fmt: skip
+    app = make_mock_index_app(index_name="root")
     yield from _utils.make_server(app)
 
 
 @pytest.fixture(scope="module")
 def mock_extra_index():
-    app = make_mock_index_app(projects={
-        "scipy": [
-            File(
-                name="scipy-1.9.0-cp310-cp310-manylinux_2_17_x86_64.whl",
-                url="spam eggs 17",
-                fragment="sha256=",
-                attributes={"data-requires-python": ">=3.7"},
-            ),
-            File(
-                name="scipy-1.9.0.tar.gz",
-                url="foo bar 17",
-                fragment="sha256=",
-                attributes={"data-requires-python": ">=3.7"},
-            ),
-        ],
-        "numpy": [
-            File(
-                name="numpy-1.23.1-cp310-cp310-macosx_10_9_x86_64.whl",
-                url="spam eggs 40c",
-                fragment="sha256=",
-                attributes={"data-requires-python": ">=3.8"},
-            ),
-        ],
-    })  # fmt: skip
+    app = make_mock_index_app(index_name="extra")
     yield from _utils.make_server(app)
 
 
 @pytest.fixture(scope="module")
 def server(mock_root_index, mock_extra_index):
     session = proxpi.server.cache.root_cache.session
     # noinspection PyProtectedMember
@@ -335,14 +237,34 @@
                 project_url, href_stripped + ".asc"
             ))
             if has_gpg_sig:
                 gpg_response.raise_for_status()
             else:
                 assert gpg_response.status_code == 404
 
+        if any(k == "data-dist-info-metadata" for k, _ in attributes):
+            (value,) = (v for k, v in attributes if k == "data-dist-info-metadata")
+            (expected,) = (v for k, v in attributes if k == "data-core-metadata")
+            assert value == expected
+
+        if any(k == "data-core-metadata" for k, _ in attributes):
+            (expected_core_metadata_hash,) = (
+                v for k, v in attributes if k == "data-core-metadata"
+            )
+            core_metadata_response = requests.get(urllib_parse.urljoin(
+                project_url, href_stripped + ".metadata"
+            ))
+            core_metadata_response.raise_for_status()
+            if expected_core_metadata_hash and expected_core_metadata_hash != "true":
+                hash_name, expected_hash_value = expected_core_metadata_hash.split("=")
+                core_metadata_hash_value = hashlib.new(
+                    hash_name, core_metadata_response.content
+                ).hexdigest()
+                assert core_metadata_hash_value == expected_hash_value
+
         if any(k == "data-requires-python" for k, _ in attributes):
             (python_requirement,) = (
                 v for k, v in attributes if k == "data-requires-python"
             )
             specifier = packaging.specifiers.SpecifierSet(python_requirement)
             assert specifier.filter(["1.2", "2.7", "3.3", "3.7", "3.10", "3.12"])
 
@@ -373,18 +295,18 @@
     """Test getting package files with JSON API."""
     params = None
     headers = None
     if query_format:
         params = {"format": accept}
     else:
         headers = {"Accept": accept}
+    project_url = f"{server}/index/{project}/"
+
     with set_mock_index_response_is_json(index_json_response):
-        response = requests.get(
-            f"{server}/index/{project}/", params=params, headers=headers
-        )
+        response = requests.get(project_url, params=params, headers=headers)
 
     assert response.status_code == 200
     assert response.headers["Content-Type"][:35] == (
         "application/vnd.pypi.simple.v1+json"
     )
     vary = {v.strip() for v in response.headers["Vary"].split(",")}
     assert "Accept-Encoding" in vary
@@ -395,14 +317,34 @@
     assert response_data["name"] == project
 
     for file in response_data["files"]:
         assert file["url"]
         assert file["filename"] == file["url"]
         assert isinstance(file["hashes"], dict)
 
+        assert not file.get("dist-info-metadata")
+
+        url_parts: urllib_parse.SplitResult = urllib_parse.urlsplit(file["url"])
+        url_parts_stripped = url_parts._replace(fragment="")
+        url_stripped = url_parts_stripped.geturl()
+        assert url_stripped == file["filename"]
+
+        if file.get("core-metadata"):
+            core_metadata_response = requests.get(
+                urllib_parse.urljoin(project_url, url_stripped + ".metadata"),
+            )
+            core_metadata_response.raise_for_status()
+
+            if isinstance(file["core-metadata"], dict):
+                for hash_name, expected_hash_value in file["core-metadata"].items():
+                    core_metadata_hash_value = hashlib.new(
+                        hash_name, core_metadata_response.content
+                    ).hexdigest()
+                    assert core_metadata_hash_value == expected_hash_value
+
     files_by_filename = {f["filename"]: f for f in response_data["files"]}
     if project == "proxpi":
         assert not files_by_filename["proxpi-1.0.0.tar.gz"].get("requires-python")
 
     elif project == "numpy":
         yanked_file = files_by_filename.pop("numpy-1.23.1-cp310-cp310-win_amd64.whl")
         assert yanked_file.get("yanked")
@@ -449,21 +391,18 @@
     response = requests.get(f"{server}/index/Jinja2/nonexistant.whl")
     assert response.status_code == 404
 
 
 @pytest.fixture
 def readonly_package_dir(tmp_path):
     package_dir = tmp_path / "packages"
-    package_dir.mkdir(mode=0o555)
+    package_dir.touch()
     with warnings.catch_warnings():
         warnings.simplefilter("ignore", pytest.PytestUnhandledThreadExceptionWarning)
-        try:
-            yield package_dir
-        finally:
-            (tmp_path / "packages").chmod(0o755)  # allow clean-up
+        yield package_dir
 
 
 def test_download_file_failed(mock_root_index, server, readonly_package_dir):
     """Test getting package file when caching failed."""
     cache_patch = mock.patch.object(proxpi_server.cache.file_cache, "_files", {})
     dir_patch = mock.patch.object(
         proxpi_server.cache.file_cache, "cache_dir", str(readonly_package_dir)
```

### Comparing `proxpi-1.2.0a0/tests/test_pypi.py` & `proxpi-1.2.0a1/tests/test_pypi.py`

 * *Files identical despite different names*

