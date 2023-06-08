# Comparing `tmp/gto-0.3.2.tar.gz` & `tmp/gto-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gto-0.3.2.tar", last modified: Wed May 31 09:42:12 2023, max compression
+gzip compressed data, was "gto-0.3.3.tar", last modified: Thu Jun  8 15:55:25 2023, max compression
```

## Comparing `gto-0.3.2.tar` & `gto-0.3.3.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:42:12.420599 gto-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-31 09:41:55.000000 gto-0.3.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:42:12.404599 gto-0.3.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:42:12.408599 gto-0.3.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-31 09:41:55.000000 gto-0.3.2/.github/ISSUE_TEMPLATE/epic-or-story.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:42:12.408599 gto-0.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-05-31 09:41:55.000000 gto-0.3.2/.github/workflows/check-test-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-31 09:41:55.000000 gto-0.3.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-31 09:41:55.000000 gto-0.3.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    20057 2023-05-31 09:41:55.000000 gto-0.3.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-05-31 09:41:55.000000 gto-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-05-31 09:42:12.420599 gto-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-05-31 09:41:55.000000 gto-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:42:12.412599 gto-0.3.2/gto/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-31 09:41:55.000000 gto-0.3.2/gto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-31 09:42:12.000000 gto-0.3.2/gto/_gto_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-31 09:41:55.000000 gto-0.3.2/gto/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16028 2023-05-31 09:41:55.000000 gto-0.3.2/gto/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19695 2023-05-31 09:41:55.000000 gto-0.3.2/gto/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    25182 2023-05-31 09:41:55.000000 gto-0.3.2/gto/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-31 09:41:55.000000 gto-0.3.2/gto/commit_message_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-05-31 09:41:55.000000 gto-0.3.2/gto/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-05-31 09:41:55.000000 gto-0.3.2/gto/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-05-31 09:41:55.000000 gto-0.3.2/gto/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-31 09:41:55.000000 gto-0.3.2/gto/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-05-31 09:41:55.000000 gto-0.3.2/gto/git_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18038 2023-05-31 09:41:55.000000 gto-0.3.2/gto/index.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-31 09:41:55.000000 gto-0.3.2/gto/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    20901 2023-05-31 09:41:55.000000 gto-0.3.2/gto/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11221 2023-05-31 09:41:55.000000 gto-0.3.2/gto/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-31 09:41:55.000000 gto-0.3.2/gto/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-31 09:41:55.000000 gto-0.3.2/gto/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-31 09:41:55.000000 gto-0.3.2/gto/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:42:12.416599 gto-0.3.2/gto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-05-31 09:42:12.000000 gto-0.3.2/gto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-31 09:42:12.000000 gto-0.3.2/gto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:42:12.000000 gto-0.3.2/gto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-31 09:42:12.000000 gto-0.3.2/gto.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:42:12.000000 gto-0.3.2/gto.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-31 09:42:12.000000 gto-0.3.2/gto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-31 09:42:12.000000 gto-0.3.2/gto.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-31 09:41:55.000000 gto-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-31 09:41:55.000000 gto-0.3.2/renovate.json
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-31 09:42:12.420599 gto-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-31 09:41:55.000000 gto-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:42:12.416599 gto-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:41:55.000000 gto-0.3.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-05-31 09:41:55.000000 gto-0.3.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:42:12.420599 gto-0.3.2/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-31 09:41:55.000000 gto-0.3.2/tests/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-31 09:41:55.000000 gto-0.3.2/tests/resources/sample_remote_repo_expected_history_churn.json
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-31 09:41:55.000000 gto-0.3.2/tests/resources/sample_remote_repo_expected_registry.json
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-31 09:41:55.000000 gto-0.3.2/tests/skip_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)    22113 2023-05-31 09:41:55.000000 gto-0.3.2/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10301 2023-05-31 09:41:55.000000 gto-0.3.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-31 09:41:55.000000 gto-0.3.2/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-31 09:41:55.000000 gto-0.3.2/tests/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13338 2023-05-31 09:41:55.000000 gto-0.3.2/tests/test_git_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-05-31 09:41:55.000000 gto-0.3.2/tests/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)    19732 2023-05-31 09:41:55.000000 gto-0.3.2/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-05-31 09:41:55.000000 gto-0.3.2/tests/test_showcase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-05-31 09:41:55.000000 gto-0.3.2/tests/test_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-31 09:41:55.000000 gto-0.3.2/tests/test_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-31 09:41:55.000000 gto-0.3.2/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:55:25.642439 gto-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-08 15:55:09.000000 gto-0.3.3/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:55:25.626438 gto-0.3.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:55:25.630438 gto-0.3.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-08 15:55:09.000000 gto-0.3.3/.github/ISSUE_TEMPLATE/epic-or-story.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:55:25.630438 gto-0.3.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-06-08 15:55:09.000000 gto-0.3.3/.github/workflows/check-test-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-08 15:55:09.000000 gto-0.3.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-08 15:55:09.000000 gto-0.3.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    20057 2023-06-08 15:55:09.000000 gto-0.3.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-06-08 15:55:09.000000 gto-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-06-08 15:55:25.642439 gto-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-06-08 15:55:09.000000 gto-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:55:25.634439 gto-0.3.3/gto/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-08 15:55:09.000000 gto-0.3.3/gto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-08 15:55:25.000000 gto-0.3.3/gto/_gto_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-08 15:55:09.000000 gto-0.3.3/gto/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16090 2023-06-08 15:55:09.000000 gto-0.3.3/gto/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19695 2023-06-08 15:55:09.000000 gto-0.3.3/gto/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25318 2023-06-08 15:55:09.000000 gto-0.3.3/gto/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-08 15:55:09.000000 gto-0.3.3/gto/commit_message_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-06-08 15:55:09.000000 gto-0.3.3/gto/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-06-08 15:55:09.000000 gto-0.3.3/gto/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-06-08 15:55:09.000000 gto-0.3.3/gto/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-08 15:55:09.000000 gto-0.3.3/gto/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-06-08 15:55:09.000000 gto-0.3.3/gto/git_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18038 2023-06-08 15:55:09.000000 gto-0.3.3/gto/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-08 15:55:09.000000 gto-0.3.3/gto/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20901 2023-06-08 15:55:09.000000 gto-0.3.3/gto/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11221 2023-06-08 15:55:09.000000 gto-0.3.3/gto/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-08 15:55:09.000000 gto-0.3.3/gto/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-06-08 15:55:09.000000 gto-0.3.3/gto/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-06-08 15:55:09.000000 gto-0.3.3/gto/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:55:25.638439 gto-0.3.3/gto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-06-08 15:55:25.000000 gto-0.3.3/gto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-08 15:55:25.000000 gto-0.3.3/gto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 15:55:25.000000 gto-0.3.3/gto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-08 15:55:25.000000 gto-0.3.3/gto.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 15:55:25.000000 gto-0.3.3/gto.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-08 15:55:25.000000 gto-0.3.3/gto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-08 15:55:25.000000 gto-0.3.3/gto.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-08 15:55:09.000000 gto-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-08 15:55:09.000000 gto-0.3.3/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-08 15:55:25.646439 gto-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-06-08 15:55:09.000000 gto-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:55:25.642439 gto-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:55:09.000000 gto-0.3.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-06-08 15:55:09.000000 gto-0.3.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:55:25.642439 gto-0.3.3/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-08 15:55:09.000000 gto-0.3.3/tests/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-08 15:55:09.000000 gto-0.3.3/tests/resources/sample_remote_repo_expected_history_churn.json
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-08 15:55:09.000000 gto-0.3.3/tests/resources/sample_remote_repo_expected_registry.json
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-08 15:55:09.000000 gto-0.3.3/tests/skip_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22113 2023-06-08 15:55:09.000000 gto-0.3.3/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10301 2023-06-08 15:55:09.000000 gto-0.3.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-06-08 15:55:09.000000 gto-0.3.3/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-08 15:55:09.000000 gto-0.3.3/tests/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13338 2023-06-08 15:55:09.000000 gto-0.3.3/tests/test_git_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-06-08 15:55:09.000000 gto-0.3.3/tests/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19732 2023-06-08 15:55:09.000000 gto-0.3.3/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-06-08 15:55:09.000000 gto-0.3.3/tests/test_showcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-06-08 15:55:09.000000 gto-0.3.3/tests/test_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-08 15:55:09.000000 gto-0.3.3/tests/test_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-08 15:55:09.000000 gto-0.3.3/tests/utils.py
```

### Comparing `gto-0.3.2/.github/ISSUE_TEMPLATE/epic-or-story.md` & `gto-0.3.3/.github/ISSUE_TEMPLATE/epic-or-story.md`

 * *Files identical despite different names*

### Comparing `gto-0.3.2/.github/workflows/check-test-release.yml` & `gto-0.3.3/.github/workflows/check-test-release.yml`

 * *Files identical despite different names*

### Comparing `gto-0.3.2/.gitignore` & `gto-0.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `gto-0.3.2/.pre-commit-config.yaml` & `gto-0.3.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `gto-0.3.2/.pylintrc` & `gto-0.3.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `gto-0.3.2/LICENSE` & `gto-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gto-0.3.2/PKG-INFO` & `gto-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gto
-Version: 0.3.2
+Version: 0.3.3
 Summary: Version and deploy your models following GitOps principles
 Download-URL: https://github.com/iterative/gto
 Author: Alexander Guschin
 Author-email: aguschin@iterative.ai
 License: Apache License 2.0
 Keywords: git repo repository artifact registry developer-tools collaboration
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `gto-0.3.2/README.md` & `gto-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `gto-0.3.2/gto/api.py` & `gto-0.3.3/gto/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,26 +206,28 @@
             author_email=author_email,
         )
 
 
 def deprecate(
     repo: Union[str, Repo],
     name: str,
-    message: str = None,
+    ref: Optional[str] = None,
+    message: Optional[str] = None,
     stdout: bool = False,
     simple: Optional[bool] = None,
     force: bool = False,
     delete: bool = False,
     push: bool = False,
     author: Optional[str] = None,
     author_email: Optional[str] = None,
 ):
     with GitRegistry.from_repo(repo) as reg:
         return reg.deprecate(
             name=name,
+            ref=ref,
             message=message,
             stdout=stdout,
             simple=simple,
             force=force,
             delete=delete,
             push=push or is_url_of_remote_repo(repo),
             author=author,
```

### Comparing `gto-0.3.2/gto/base.py` & `gto-0.3.3/gto/base.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.2/gto/cli.py` & `gto-0.3.3/gto/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -575,14 +575,17 @@
 
 @gto_command(section=CommandGroups.modifying)
 def deprecate(
     repo: str = option_repo,
     name: str = arg_name,
     version: str = Argument(None, help="Artifact version"),
     stage: str = Argument(None, help="Stage to unassign"),
+    ref: Optional[str] = Option(
+        None, "--ref", help="Git reference to use (for model deprecation)"
+    ),
     message: Optional[str] = option_message,
     simple: str = option_simple,
     force: bool = option_force,
     delete: bool = option_delete,
     push: bool = option_push_tag,
 ):
     """Deprecate artifact, deregister a version, or unassign a stage."""
@@ -611,14 +614,15 @@
             push=push,
             stdout=True,
         )
     else:
         gto.api.deprecate(
             repo=repo,
             name=name,
+            ref=ref,
             message=message,
             simple=simple,  # type: ignore
             force=force,
             delete=delete,
             push=push,
             stdout=True,
         )
```

### Comparing `gto-0.3.2/gto/config.py` & `gto-0.3.3/gto/config.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.2/gto/constants.py` & `gto-0.3.3/gto/constants.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.2/gto/exceptions.py` & `gto-0.3.3/gto/exceptions.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.2/gto/ext.py` & `gto-0.3.3/gto/ext.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.2/gto/git_utils.py` & `gto-0.3.3/gto/git_utils.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.2/gto/index.py` & `gto-0.3.3/gto/index.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.2/gto/log.py` & `gto-0.3.3/gto/log.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.2/gto/registry.py` & `gto-0.3.3/gto/registry.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.2/gto/tag.py` & `gto-0.3.3/gto/tag.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.2/gto/ui.py` & `gto-0.3.3/gto/ui.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.2/gto/utils.py` & `gto-0.3.3/gto/utils.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.2/gto/versions.py` & `gto-0.3.3/gto/versions.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.2/gto.egg-info/PKG-INFO` & `gto-0.3.3/gto.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gto
-Version: 0.3.2
+Version: 0.3.3
 Summary: Version and deploy your models following GitOps principles
 Download-URL: https://github.com/iterative/gto
 Author: Alexander Guschin
 Author-email: aguschin@iterative.ai
 License: Apache License 2.0
 Keywords: git repo repository artifact registry developer-tools collaboration
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `gto-0.3.2/gto.egg-info/SOURCES.txt` & `gto-0.3.3/gto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gto-0.3.2/setup.cfg` & `gto-0.3.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `gto-0.3.2/setup.py` & `gto-0.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.2/tests/conftest.py` & `gto-0.3.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.2/tests/resources/__init__.py` & `gto-0.3.3/tests/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.2/tests/resources/sample_remote_repo_expected_history_churn.json` & `gto-0.3.3/tests/resources/sample_remote_repo_expected_history_churn.json`

 * *Files identical despite different names*

### Comparing `gto-0.3.2/tests/resources/sample_remote_repo_expected_registry.json` & `gto-0.3.3/tests/resources/sample_remote_repo_expected_registry.json`

 * *Files identical despite different names*

### Comparing `gto-0.3.2/tests/skip_presets.py` & `gto-0.3.3/tests/skip_presets.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.2/tests/test_api.py` & `gto-0.3.3/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.2/tests/test_cli.py` & `gto-0.3.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.2/tests/test_config.py` & `gto-0.3.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.2/tests/test_constants.py` & `gto-0.3.3/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.2/tests/test_git_utils.py` & `gto-0.3.3/tests/test_git_utils.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.2/tests/test_index.py` & `gto-0.3.3/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.2/tests/test_registry.py` & `gto-0.3.3/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.2/tests/test_showcase.py` & `gto-0.3.3/tests/test_showcase.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.2/tests/test_tag.py` & `gto-0.3.3/tests/test_tag.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.2/tests/test_versions.py` & `gto-0.3.3/tests/test_versions.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.2/tests/utils.py` & `gto-0.3.3/tests/utils.py`

 * *Files identical despite different names*

