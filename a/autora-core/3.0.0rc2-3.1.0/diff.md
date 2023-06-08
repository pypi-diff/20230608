# Comparing `tmp/autora-core-3.0.0rc2.tar.gz` & `tmp/autora-core-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-core-3.0.0rc2.tar", last modified: Thu Jun  1 19:38:49 2023, max compression
+gzip compressed data, was "autora-core-3.1.0.tar", last modified: Thu Jun  8 14:55:37 2023, max compression
```

## Comparing `autora-core-3.0.0rc2.tar` & `autora-core-3.1.0.tar`

### file list

```diff
@@ -1,68 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:49.401503 autora-core-3.0.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:49.397503 autora-core-3.0.0rc2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:49.397503 autora-core-3.0.0rc2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/.github/workflows/publish-package-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/.github/workflows/test-pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:49.401503 autora-core-3.0.0rc2/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/.idea/autora-core.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:49.401503 autora-core-3.0.0rc2/.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/.idea/codeStyles/codeStyleConfig.xml
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/.idea/encodings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:49.401503 autora-core-3.0.0rc2/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/.idea/other.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:49.401503 autora-core-3.0.0rc2/.idea/runConfigurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/.idea/runConfigurations/pytest.xml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:49.401503 autora-core-3.0.0rc2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/.vscode/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/CONTRIBUTE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-01 19:38:49.401503 autora-core-3.0.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:49.401503 autora-core-3.0.0rc2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:49.401503 autora-core-3.0.0rc2/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/docs/javascripts/mathjax.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:49.401503 autora-core-3.0.0rc2/docs/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/docs/pipeline/Experimentalist Pipeline Examples.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:49.401503 autora-core-3.0.0rc2/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 19:38:49.401503 autora-core-3.0.0rc2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:49.397503 autora-core-3.0.0rc2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:49.397503 autora-core-3.0.0rc2/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:49.401503 autora-core-3.0.0rc2/src/autora/experimentalist/
--rw-r--r--   0 runner    (1001) docker     (123)    18310 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/src/autora/experimentalist/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:49.401503 autora-core-3.0.0rc2/src/autora/experimentalist/pooler/
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/src/autora/experimentalist/pooler/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/src/autora/experimentalist/pooler/random_pooler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:49.401503 autora-core-3.0.0rc2/src/autora/experimentalist/sampler/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/src/autora/experimentalist/sampler/random_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/src/autora/experimentalist/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:49.401503 autora-core-3.0.0rc2/src/autora/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/src/autora/utils/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:49.401503 autora-core-3.0.0rc2/src/autora/variable/
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/src/autora/variable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/src/autora/variable/time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:49.401503 autora-core-3.0.0rc2/src/autora_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-01 19:38:49.000000 autora-core-3.0.0rc2/src/autora_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-01 19:38:49.000000 autora-core-3.0.0rc2/src/autora_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 19:38:49.000000 autora-core-3.0.0rc2/src/autora_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-01 19:38:49.000000 autora-core-3.0.0rc2/src/autora_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-01 19:38:49.000000 autora-core-3.0.0rc2/src/autora_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:49.401503 autora-core-3.0.0rc2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/tests/test_experimentalist_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/tests/test_experimentalist_random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:55:37.663045 autora-core-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-08 14:55:27.000000 autora-core-3.1.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:55:37.659045 autora-core-3.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-08 14:55:27.000000 autora-core-3.1.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:55:37.659045 autora-core-3.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-08 14:55:27.000000 autora-core-3.1.0/.github/workflows/publish-package-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-08 14:55:27.000000 autora-core-3.1.0/.github/workflows/test-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-08 14:55:27.000000 autora-core-3.1.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:55:37.659045 autora-core-3.1.0/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-08 14:55:27.000000 autora-core-3.1.0/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-08 14:55:27.000000 autora-core-3.1.0/.idea/autora-core.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:55:37.659045 autora-core-3.1.0/.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-08 14:55:27.000000 autora-core-3.1.0/.idea/codeStyles/codeStyleConfig.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-08 14:55:27.000000 autora-core-3.1.0/.idea/encodings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:55:37.659045 autora-core-3.1.0/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-08 14:55:27.000000 autora-core-3.1.0/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-08 14:55:27.000000 autora-core-3.1.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-08 14:55:27.000000 autora-core-3.1.0/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-08 14:55:27.000000 autora-core-3.1.0/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-08 14:55:27.000000 autora-core-3.1.0/.idea/other.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:55:37.659045 autora-core-3.1.0/.idea/runConfigurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-08 14:55:27.000000 autora-core-3.1.0/.idea/runConfigurations/pytest.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-08 14:55:27.000000 autora-core-3.1.0/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-08 14:55:27.000000 autora-core-3.1.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:55:37.659045 autora-core-3.1.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 14:55:27.000000 autora-core-3.1.0/.vscode/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-08 14:55:27.000000 autora-core-3.1.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-08 14:55:27.000000 autora-core-3.1.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-08 14:55:27.000000 autora-core-3.1.0/CONTRIBUTE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-08 14:55:27.000000 autora-core-3.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-08 14:55:37.663045 autora-core-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-08 14:55:27.000000 autora-core-3.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:55:37.659045 autora-core-3.1.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:55:37.655045 autora-core-3.1.0/docs/experimentalists/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:55:37.655045 autora-core-3.1.0/docs/experimentalists/pooler/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:55:37.659045 autora-core-3.1.0/docs/experimentalists/pooler/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-08 14:55:27.000000 autora-core-3.1.0/docs/experimentalists/pooler/grid/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-08 14:55:27.000000 autora-core-3.1.0/docs/experimentalists/pooler/grid/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:55:37.663045 autora-core-3.1.0/docs/experimentalists/pooler/random/
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-08 14:55:27.000000 autora-core-3.1.0/docs/experimentalists/pooler/random/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-08 14:55:27.000000 autora-core-3.1.0/docs/experimentalists/pooler/random/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:55:37.655045 autora-core-3.1.0/docs/experimentalists/sampler/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:55:37.663045 autora-core-3.1.0/docs/experimentalists/sampler/random/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-08 14:55:27.000000 autora-core-3.1.0/docs/experimentalists/sampler/random/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-08 14:55:27.000000 autora-core-3.1.0/docs/experimentalists/sampler/random/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-08 14:55:27.000000 autora-core-3.1.0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:55:37.663045 autora-core-3.1.0/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-08 14:55:27.000000 autora-core-3.1.0/docs/javascripts/mathjax.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:55:37.663045 autora-core-3.1.0/docs/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-06-08 14:55:27.000000 autora-core-3.1.0/docs/pipeline/Experimentalist Pipeline Examples.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:55:37.663045 autora-core-3.1.0/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-08 14:55:27.000000 autora-core-3.1.0/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-08 14:55:27.000000 autora-core-3.1.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-08 14:55:27.000000 autora-core-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 14:55:37.663045 autora-core-3.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:55:37.659045 autora-core-3.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:55:37.659045 autora-core-3.1.0/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:55:37.663045 autora-core-3.1.0/src/autora/experimentalist/
+-rw-r--r--   0 runner    (1001) docker     (123)    18310 2023-06-08 14:55:27.000000 autora-core-3.1.0/src/autora/experimentalist/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:55:37.663045 autora-core-3.1.0/src/autora/experimentalist/pooler/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-08 14:55:27.000000 autora-core-3.1.0/src/autora/experimentalist/pooler/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-08 14:55:27.000000 autora-core-3.1.0/src/autora/experimentalist/pooler/random_pooler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:55:37.663045 autora-core-3.1.0/src/autora/experimentalist/sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-08 14:55:27.000000 autora-core-3.1.0/src/autora/experimentalist/sampler/random_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-06-08 14:55:27.000000 autora-core-3.1.0/src/autora/experimentalist/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:55:37.663045 autora-core-3.1.0/src/autora/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-08 14:55:27.000000 autora-core-3.1.0/src/autora/utils/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-08 14:55:27.000000 autora-core-3.1.0/src/autora/utils/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:55:37.663045 autora-core-3.1.0/src/autora/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-08 14:55:27.000000 autora-core-3.1.0/src/autora/variable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-06-08 14:55:27.000000 autora-core-3.1.0/src/autora/variable/time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:55:37.663045 autora-core-3.1.0/src/autora_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-08 14:55:37.000000 autora-core-3.1.0/src/autora_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-08 14:55:37.000000 autora-core-3.1.0/src/autora_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 14:55:37.000000 autora-core-3.1.0/src/autora_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-08 14:55:37.000000 autora-core-3.1.0/src/autora_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 14:55:37.000000 autora-core-3.1.0/src/autora_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:55:37.663045 autora-core-3.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-08 14:55:27.000000 autora-core-3.1.0/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-06-08 14:55:27.000000 autora-core-3.1.0/tests/test_experimentalist_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-06-08 14:55:27.000000 autora-core-3.1.0/tests/test_experimentalist_random.py
```

### Comparing `autora-core-3.0.0rc2/.github/pull_request_template.md` & `autora-core-3.1.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0rc2/.github/workflows/publish-package-pypi.yml` & `autora-core-3.1.0/.github/workflows/publish-package-pypi.yml`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0rc2/.github/workflows/test-pytest.yml` & `autora-core-3.1.0/.github/workflows/test-pytest.yml`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0rc2/.gitignore` & `autora-core-3.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0rc2/.idea/autora-core.iml` & `autora-core-3.1.0/.idea/autora-core.iml`

 * *Files 2% similar despite different names*

#### Comparing `autora-core-3.0.0rc2/.idea/autora-core.iml` & `autora-core-3.1.0/.idea/autora-core.iml`

```diff
@@ -23,13 +23,12 @@
     <option name="myDocStringFormat" value="Google"/>
     <option name="renderExternalDocumentation" value="true"/>
   </component>
   <component name="PyNamespacePackagesService">
     <option name="namespacePackageFolders">
       <list>
         <option value="$MODULE_DIR$/src/autora"/>
-        <option value="$MODULE_DIR$/src/autora/synthetic"/>
         <option value="$MODULE_DIR$/src/autora/experimentalist"/>
       </list>
     </option>
   </component>
 </module>
```

### Comparing `autora-core-3.0.0rc2/.idea/inspectionProfiles/Project_Default.xml` & `autora-core-3.1.0/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0rc2/.idea/runConfigurations/pytest.xml` & `autora-core-3.1.0/.idea/runConfigurations/pytest.xml`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0rc2/.pre-commit-config.yaml` & `autora-core-3.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0rc2/CONTRIBUTE.md` & `autora-core-3.1.0/CONTRIBUTE.md`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0rc2/LICENSE.md` & `autora-core-3.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0rc2/PKG-INFO` & `autora-core-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-core
-Version: 3.0.0rc2
+Version: 3.1.0
 Summary: Autonomous Research Assistant (AutoRA) is a framework for automating steps of the empirical research process. 
 Author-email: Sebastian Musslick <sebastian_musslick@brown.edu>, John Gerrard Holland <john_holland1@brown.edu>
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-core
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
```

### Comparing `autora-core-3.0.0rc2/README.md` & `autora-core-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0rc2/docs/pipeline/Experimentalist Pipeline Examples.ipynb` & `autora-core-3.1.0/docs/pipeline/Experimentalist Pipeline Examples.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999092261904762%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(5, 'from autora.experimentalist.sampler.random_sampler "*

 * *            "import random_sample')], delete: [5]}}, 8: {'source': {insert: [(7, '    "*

 * *            '("random_sample", random_sample)\\n\'), (9, \'    {"grid_pool": {"ivs": '*

 * *            'metadata.independent_variables}, "random_sample": {"n": 10}}\\n\')], delete: [9, '*

 * *            '7]}}, 12: {\'source\': {insert: [(9, \'        ("sample", random_sample) # Sampler '*

 * *            'defined in the first implementatio […]*

```diff
@@ -30,15 +30,15 @@
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "\n",
                 "from autora.variable import DV, IV, ValueType, VariableCollection\n",
                 "from autora.experimentalist.pipeline import Pipeline\n",
                 "from autora.experimentalist.pooler.grid import grid_pool\n",
-                "from autora.experimentalist.sampler.random_sampler import random_sampler"
+                "from autora.experimentalist.sampler.random_sampler import random_sample"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -141,17 +141,17 @@
                 "## Set up pipeline functions with the partial function\n",
                 "# Random Sampler\n",
                 "\n",
                 "# Initialize the pipeline\n",
                 "pipeline_random_samp = Pipeline([\n",
                 "    (\"grid_pool\", grid_pool),\n",
                 "    (\"weber_filer\", weber_filter), # Filter that selects conditions with IV1 <= IV2\n",
-                "    (\"random_sampler\", random_sampler)\n",
+                "    (\"random_sample\", random_sample)\n",
                 "],\n",
-                "    {\"grid_pool\": {\"ivs\": metadata.independent_variables}, \"random_sampler\": {\"n\": 10}}\n",
+                "    {\"grid_pool\": {\"ivs\": metadata.independent_variables}, \"random_sample\": {\"n\": 10}}\n",
                 ")\n",
                 "pipeline_random_samp"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -213,17 +213,17 @@
                 "pooler_iterator = grid_pool(metadata.independent_variables)\n",
                 "\n",
                 "# Initialize the pipeline\n",
                 "pipeline_random_samp2 = Pipeline(\n",
                 "    [\n",
                 "        (\"pool (iterator)\", pooler_iterator),\n",
                 "        (\"filter\",weber_filter), # Filter that selects conditions with IV1 <= IV2\n",
-                "        (\"sampler\", random_sampler) # Sampler defined in the first implementation example\n",
+                "        (\"sample\", random_sample) # Sampler defined in the first implementation example\n",
                 "    ],\n",
-                "    {\"sampler\": {\"n\": 10}}\n",
+                "    {\"sample\": {\"n\": 10}}\n",
                 ")\n",
                 "# Run the Pipeline\n",
                 "results1 = pipeline_random_samp2.run()\n",
                 "results2 = pipeline_random_samp2.run()\n",
                 "print('Sampled Conditions:')\n",
                 "print(f' Run 1: {results1}\\n',\n",
                 "      f'Run 2: {results2}')"
@@ -259,17 +259,17 @@
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "pipeline_random_samp = Pipeline([\n",
                 "    (\"grid_pool\", grid_pool),\n",
                 "    (\"weber_filer\", weber_filter), # Filter that selects conditions with IV1 <= IV2\n",
-                "    (\"random_sampler\", random_sampler)\n",
+                "    (\"random_sample\", random_sample)\n",
                 "],\n",
-                "    {\"grid_pool__ivs\": metadata.independent_variables, \"random_sampler__n\": 10}\n",
+                "    {\"grid_pool__ivs\": metadata.independent_variables, \"random_sample__n\": 10}\n",
                 ")\n",
                 "pipeline_random_samp\n"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
```

### Comparing `autora-core-3.0.0rc2/mkdocs/base.yml` & `autora-core-3.1.0/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0rc2/pyproject.toml` & `autora-core-3.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0rc2/src/autora/experimentalist/pipeline.py` & `autora-core-3.1.0/src/autora/experimentalist/pipeline.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0rc2/src/autora/experimentalist/pooler/grid.py` & `autora-core-3.1.0/src/autora/experimentalist/pooler/grid.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0rc2/src/autora/experimentalist/pooler/random_pooler.py` & `autora-core-3.1.0/src/autora/experimentalist/pooler/random_pooler.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import random
 
 import numpy as np
 
+from autora.utils.deprecation import deprecated_alias
 
-def random_pool(*args, n=1, duplicates=True):
+
+def random_pool(*args, n: int = 1, duplicates: bool = True):
     """
     Creates combinations from lists of discrete values using random selection.
     Args:
         *args: m lists of discrete values. One value will be sampled from each list.
         n: Number of samples to sample
         duplicates: Boolean if duplicate value are allowed.
 
@@ -31,7 +33,10 @@
     # Random sample from the pools until n is met
     while len(l_samples) < n:
         l_samples.append(tuple(map(random.choice, pools)))
         if not duplicates:
             l_samples = [*set(l_samples)]
 
     return iter(l_samples)
+
+
+random_pooler = deprecated_alias(random_pool, "random_pooler")
```

### Comparing `autora-core-3.0.0rc2/src/autora/experimentalist/utils.py` & `autora-core-3.1.0/src/autora/experimentalist/utils.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0rc2/src/autora/variable/__init__.py` & `autora-core-3.1.0/src/autora/variable/__init__.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0rc2/src/autora/variable/time.py` & `autora-core-3.1.0/src/autora/variable/time.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0rc2/src/autora_core.egg-info/PKG-INFO` & `autora-core-3.1.0/src/autora_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-core
-Version: 3.0.0rc2
+Version: 3.1.0
 Summary: Autonomous Research Assistant (AutoRA) is a framework for automating steps of the empirical research process. 
 Author-email: Sebastian Musslick <sebastian_musslick@brown.edu>, John Gerrard Holland <john_holland1@brown.edu>
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-core
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
```

### Comparing `autora-core-3.0.0rc2/src/autora_core.egg-info/SOURCES.txt` & `autora-core-3.1.0/src/autora_core.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -20,22 +20,29 @@
 .idea/inspectionProfiles/Project_Default.xml
 .idea/inspectionProfiles/profiles_settings.xml
 .idea/runConfigurations/pytest.xml
 .vscode/.gitignore
 .vscode/extensions.json
 .vscode/launch.json
 docs/index.md
+docs/experimentalists/pooler/grid/index.md
+docs/experimentalists/pooler/grid/quickstart.md
+docs/experimentalists/pooler/random/index.md
+docs/experimentalists/pooler/random/quickstart.md
+docs/experimentalists/sampler/random/index.md
+docs/experimentalists/sampler/random/quickstart.md
 docs/javascripts/mathjax.js
 docs/pipeline/Experimentalist Pipeline Examples.ipynb
 mkdocs/base.yml
 src/autora/experimentalist/pipeline.py
 src/autora/experimentalist/utils.py
 src/autora/experimentalist/pooler/grid.py
 src/autora/experimentalist/pooler/random_pooler.py
 src/autora/experimentalist/sampler/random_sampler.py
+src/autora/utils/deprecation.py
 src/autora/utils/dictionary.py
 src/autora/variable/__init__.py
 src/autora/variable/time.py
 src/autora_core.egg-info/PKG-INFO
 src/autora_core.egg-info/SOURCES.txt
 src/autora_core.egg-info/dependency_links.txt
 src/autora_core.egg-info/requires.txt
```

### Comparing `autora-core-3.0.0rc2/tests/README.md` & `autora-core-3.1.0/tests/README.md`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0rc2/tests/test_experimentalist_pipeline.py` & `autora-core-3.1.0/tests/test_experimentalist_pipeline.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0rc2/tests/test_experimentalist_random.py` & `autora-core-3.1.0/tests/test_experimentalist_random.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from functools import partial
 
 import numpy as np
 import pytest
 
 from autora.experimentalist.pipeline import make_pipeline
 from autora.experimentalist.pooler.grid import grid_pool
-from autora.experimentalist.sampler.random_sampler import random_sampler
+from autora.experimentalist.sampler.random_sampler import random_sample
 from autora.variable import DV, IV, ValueType, VariableCollection
 
 
 def weber_filter(values):
     return filter(lambda s: s[0] <= s[1], values)
 
 
@@ -22,15 +22,15 @@
     """
 
     n_trials = 25  # Number of trails for sampler to select
 
     # ---Implementation 1 - Pool using Callable via partial function----
     # Set up pipeline functions with partial
     pooler_callable = partial(grid_pool, ivs=metadata.independent_variables)
-    sampler = partial(random_sampler, n=n_trials)
+    sampler = partial(random_sample, n=n_trials)
     pipeline_random_samp = make_pipeline(
         [pooler_callable, weber_filter, sampler],
     )
 
     results = pipeline_random_samp.run()
 
     # ***Checks***
@@ -60,15 +60,15 @@
     )
 
 
 def test_random_experimentalist_generator(metadata):
     n_trials = 25  # Number of trails for sampler to select
 
     pooler_generator = grid_pool(metadata.independent_variables)
-    sampler = partial(random_sampler, n=n_trials)
+    sampler = partial(random_sample, n=n_trials)
     pipeline_random_samp_poolgen = make_pipeline(
         [pooler_generator, weber_filter, sampler]
     )
 
     results_poolgen = list(pipeline_random_samp_poolgen.run())
 
     # Is sampling the number of trials we expect
```

