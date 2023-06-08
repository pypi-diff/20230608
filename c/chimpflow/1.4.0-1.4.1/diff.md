# Comparing `tmp/chimpflow-1.4.0.tar.gz` & `tmp/chimpflow-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chimpflow-1.4.0.tar", last modified: Tue Jun  6 11:26:25 2023, max compression
+gzip compressed data, was "chimpflow-1.4.1.tar", last modified: Thu Jun  8 13:34:27 2023, max compression
```

## Comparing `chimpflow-1.4.0.tar` & `chimpflow-1.4.1.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.060840 chimpflow-1.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.020843 chimpflow-1.4.0/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.024843 chimpflow-1.4.0/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.dae-devops/docs/documenting.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.024843 chimpflow-1.4.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.024843 chimpflow-1.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.008844 chimpflow-1.4.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.028843 chimpflow-1.4.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.028843 chimpflow-1.4.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.028843 chimpflow-1.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6887 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.028843 chimpflow-1.4.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-06 11:26:13.000000 chimpflow-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14342 2023-06-06 11:26:25.060840 chimpflow-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-06 11:26:13.000000 chimpflow-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.032842 chimpflow-1.4.0/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-06 11:26:13.000000 chimpflow-1.4.0/configurations/development.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.032842 chimpflow-1.4.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.012844 chimpflow-1.4.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.032842 chimpflow-1.4.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-06 11:26:13.000000 chimpflow-1.4.0/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-06-06 11:26:13.000000 chimpflow-1.4.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.032842 chimpflow-1.4.0/docs/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-06 11:26:13.000000 chimpflow-1.4.0/docs/explanations/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-06 11:26:13.000000 chimpflow-1.4.0/docs/explanations/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-06 11:26:13.000000 chimpflow-1.4.0/docs/explanations/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-06 11:26:13.000000 chimpflow-1.4.0/docs/explanations/todo.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.036842 chimpflow-1.4.0/docs/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-06 11:26:13.000000 chimpflow-1.4.0/docs/how-to/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-06 11:26:13.000000 chimpflow-1.4.0/docs/how-to/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-06 11:26:13.000000 chimpflow-1.4.0/docs/how-to/documenting.rst
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-06 11:26:13.000000 chimpflow-1.4.0/docs/how-to/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-06 11:26:13.000000 chimpflow-1.4.0/docs/how-to/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-06 11:26:13.000000 chimpflow-1.4.0/docs/how-to/testing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.036842 chimpflow-1.4.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-06-06 11:26:13.000000 chimpflow-1.4.0/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-06 11:26:13.000000 chimpflow-1.4.0/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-06 11:26:13.000000 chimpflow-1.4.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.036842 chimpflow-1.4.0/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-06 11:26:13.000000 chimpflow-1.4.0/docs/reference/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-06 11:26:13.000000 chimpflow-1.4.0/docs/reference/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-06 11:26:13.000000 chimpflow-1.4.0/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-06 11:26:13.000000 chimpflow-1.4.0/docs/reference/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.040842 chimpflow-1.4.0/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-06 11:26:13.000000 chimpflow-1.4.0/docs/tutorials/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-06 11:26:13.000000 chimpflow-1.4.0/docs/tutorials/tbd.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-06-06 11:26:13.000000 chimpflow-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 11:26:25.060840 chimpflow-1.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.016843 chimpflow-1.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.040842 chimpflow-1.4.0/src/chimpflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14342 2023-06-06 11:26:24.000000 chimpflow-1.4.0/src/chimpflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-06-06 11:26:25.000000 chimpflow-1.4.0/src/chimpflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 11:26:24.000000 chimpflow-1.4.0/src/chimpflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-06 11:26:24.000000 chimpflow-1.4.0/src/chimpflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-06 11:26:24.000000 chimpflow-1.4.0/src/chimpflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-06 11:26:24.000000 chimpflow-1.4.0/src/chimpflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.044841 chimpflow-1.4.0/src/chimpflow_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_api/aiohttp_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_api/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.044841 chimpflow-1.4.0/src/chimpflow_api/miners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_api/miners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_api/miners/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_api/miners/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_api/miners/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_api/miners/miners.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_api/thing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_api/things.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.048841 chimpflow-1.4.0/src/chimpflow_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.048841 chimpflow-1.4.0/src/chimpflow_cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_cli/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_cli/subcommands/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.052841 chimpflow-1.4.0/src/chimpflow_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-06 11:26:24.000000 chimpflow-1.4.0/src/chimpflow_lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_lib/base_aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10171 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_lib/chimp_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_lib/envvar.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_lib/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.056841 chimpflow-1.4.0/src/chimpflow_lib/miners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_lib/miners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_lib/miners/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_lib/miners/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_lib/miners/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_lib/miners/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_lib/miners/direct_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_lib/miners/miners.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.056841 chimpflow-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:13.000000 chimpflow-1.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-06-06 11:26:13.000000 chimpflow-1.4.0/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.056841 chimpflow-1.4.0/tests/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-06 11:26:13.000000 chimpflow-1.4.0/tests/configurations/direct_sqlite.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-06 11:26:13.000000 chimpflow-1.4.0/tests/configurations/service_mysql.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-06-06 11:26:13.000000 chimpflow-1.4.0/tests/configurations/service_sqlite.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-06-06 11:26:13.000000 chimpflow-1.4.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.056841 chimpflow-1.4.0/tests/echo_test_imgs/
--rw-r--r--   0 runner    (1001) docker     (123)   156218 2023-06-06 11:26:13.000000 chimpflow-1.4.0/tests/echo_test_imgs/97wo_01A_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   146361 2023-06-06 11:26:13.000000 chimpflow-1.4.0/tests/echo_test_imgs/97wo_01A_2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   142418 2023-06-06 11:26:13.000000 chimpflow-1.4.0/tests/echo_test_imgs/97wo_01A_3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-06-06 11:26:13.000000 chimpflow-1.4.0/tests/test_chimp_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-06-06 11:26:13.000000 chimpflow-1.4.0/tests/test_miner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:34:27.260926 chimpflow-1.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:34:27.240926 chimpflow-1.4.1/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-08 13:34:14.000000 chimpflow-1.4.1/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:34:27.244926 chimpflow-1.4.1/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-08 13:34:14.000000 chimpflow-1.4.1/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-08 13:34:14.000000 chimpflow-1.4.1/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-06-08 13:34:14.000000 chimpflow-1.4.1/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-08 13:34:14.000000 chimpflow-1.4.1/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-08 13:34:14.000000 chimpflow-1.4.1/.dae-devops/docs/documenting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-08 13:34:14.000000 chimpflow-1.4.1/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-08 13:34:14.000000 chimpflow-1.4.1/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-08 13:34:14.000000 chimpflow-1.4.1/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-08 13:34:14.000000 chimpflow-1.4.1/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:34:27.244926 chimpflow-1.4.1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-08 13:34:14.000000 chimpflow-1.4.1/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-06-08 13:34:14.000000 chimpflow-1.4.1/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:34:27.244926 chimpflow-1.4.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-08 13:34:14.000000 chimpflow-1.4.1/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:34:27.236926 chimpflow-1.4.1/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:34:27.244926 chimpflow-1.4.1/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-06-08 13:34:14.000000 chimpflow-1.4.1/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-08 13:34:14.000000 chimpflow-1.4.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:34:27.244926 chimpflow-1.4.1/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-08 13:34:14.000000 chimpflow-1.4.1/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-08 13:34:14.000000 chimpflow-1.4.1/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:34:27.244926 chimpflow-1.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6887 2023-06-08 13:34:14.000000 chimpflow-1.4.1/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-08 13:34:14.000000 chimpflow-1.4.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-08 13:34:14.000000 chimpflow-1.4.1/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-08 13:34:14.000000 chimpflow-1.4.1/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-08 13:34:14.000000 chimpflow-1.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-08 13:34:14.000000 chimpflow-1.4.1/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-08 13:34:14.000000 chimpflow-1.4.1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:34:27.244926 chimpflow-1.4.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-08 13:34:14.000000 chimpflow-1.4.1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-08 13:34:14.000000 chimpflow-1.4.1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-08 13:34:14.000000 chimpflow-1.4.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-08 13:34:14.000000 chimpflow-1.4.1/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-08 13:34:14.000000 chimpflow-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14342 2023-06-08 13:34:27.260926 chimpflow-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-08 13:34:14.000000 chimpflow-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:34:27.244926 chimpflow-1.4.1/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-08 13:34:14.000000 chimpflow-1.4.1/configurations/development.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:34:27.248926 chimpflow-1.4.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:34:27.240926 chimpflow-1.4.1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:34:27.248926 chimpflow-1.4.1/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-08 13:34:14.000000 chimpflow-1.4.1/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-06-08 13:34:14.000000 chimpflow-1.4.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:34:27.248926 chimpflow-1.4.1/docs/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-08 13:34:14.000000 chimpflow-1.4.1/docs/explanations/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-08 13:34:14.000000 chimpflow-1.4.1/docs/explanations/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-08 13:34:14.000000 chimpflow-1.4.1/docs/explanations/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-08 13:34:14.000000 chimpflow-1.4.1/docs/explanations/todo.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:34:27.248926 chimpflow-1.4.1/docs/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-08 13:34:14.000000 chimpflow-1.4.1/docs/how-to/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-08 13:34:14.000000 chimpflow-1.4.1/docs/how-to/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-08 13:34:14.000000 chimpflow-1.4.1/docs/how-to/documenting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-08 13:34:14.000000 chimpflow-1.4.1/docs/how-to/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-08 13:34:14.000000 chimpflow-1.4.1/docs/how-to/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-08 13:34:14.000000 chimpflow-1.4.1/docs/how-to/testing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:34:27.248926 chimpflow-1.4.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-06-08 13:34:14.000000 chimpflow-1.4.1/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-08 13:34:14.000000 chimpflow-1.4.1/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-08 13:34:14.000000 chimpflow-1.4.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:34:27.248926 chimpflow-1.4.1/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-08 13:34:14.000000 chimpflow-1.4.1/docs/reference/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-08 13:34:14.000000 chimpflow-1.4.1/docs/reference/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-08 13:34:14.000000 chimpflow-1.4.1/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-08 13:34:14.000000 chimpflow-1.4.1/docs/reference/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:34:27.252926 chimpflow-1.4.1/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-08 13:34:14.000000 chimpflow-1.4.1/docs/tutorials/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-08 13:34:14.000000 chimpflow-1.4.1/docs/tutorials/tbd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-06-08 13:34:14.000000 chimpflow-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 13:34:27.260926 chimpflow-1.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:34:27.240926 chimpflow-1.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:34:27.252926 chimpflow-1.4.1/src/chimpflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14342 2023-06-08 13:34:27.000000 chimpflow-1.4.1/src/chimpflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-06-08 13:34:27.000000 chimpflow-1.4.1/src/chimpflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 13:34:27.000000 chimpflow-1.4.1/src/chimpflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-08 13:34:27.000000 chimpflow-1.4.1/src/chimpflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-08 13:34:27.000000 chimpflow-1.4.1/src/chimpflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-08 13:34:27.000000 chimpflow-1.4.1/src/chimpflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:34:27.252926 chimpflow-1.4.1/src/chimpflow_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 13:34:14.000000 chimpflow-1.4.1/src/chimpflow_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-08 13:34:14.000000 chimpflow-1.4.1/src/chimpflow_api/aiohttp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-08 13:34:14.000000 chimpflow-1.4.1/src/chimpflow_api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-08 13:34:14.000000 chimpflow-1.4.1/src/chimpflow_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:34:27.252926 chimpflow-1.4.1/src/chimpflow_api/miners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 13:34:14.000000 chimpflow-1.4.1/src/chimpflow_api/miners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-06-08 13:34:14.000000 chimpflow-1.4.1/src/chimpflow_api/miners/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-08 13:34:14.000000 chimpflow-1.4.1/src/chimpflow_api/miners/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-08 13:34:14.000000 chimpflow-1.4.1/src/chimpflow_api/miners/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-08 13:34:14.000000 chimpflow-1.4.1/src/chimpflow_api/miners/miners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-06-08 13:34:14.000000 chimpflow-1.4.1/src/chimpflow_api/thing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-06-08 13:34:14.000000 chimpflow-1.4.1/src/chimpflow_api/things.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:34:27.252926 chimpflow-1.4.1/src/chimpflow_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-08 13:34:14.000000 chimpflow-1.4.1/src/chimpflow_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-06-08 13:34:14.000000 chimpflow-1.4.1/src/chimpflow_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:34:27.256926 chimpflow-1.4.1/src/chimpflow_cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 13:34:14.000000 chimpflow-1.4.1/src/chimpflow_cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-06-08 13:34:14.000000 chimpflow-1.4.1/src/chimpflow_cli/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-08 13:34:14.000000 chimpflow-1.4.1/src/chimpflow_cli/subcommands/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-08 13:34:14.000000 chimpflow-1.4.1/src/chimpflow_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:34:27.256926 chimpflow-1.4.1/src/chimpflow_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-08 13:34:14.000000 chimpflow-1.4.1/src/chimpflow_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-08 13:34:14.000000 chimpflow-1.4.1/src/chimpflow_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-08 13:34:27.000000 chimpflow-1.4.1/src/chimpflow_lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-08 13:34:14.000000 chimpflow-1.4.1/src/chimpflow_lib/base_aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10171 2023-06-08 13:34:14.000000 chimpflow-1.4.1/src/chimpflow_lib/chimp_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-08 13:34:14.000000 chimpflow-1.4.1/src/chimpflow_lib/envvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-08 13:34:14.000000 chimpflow-1.4.1/src/chimpflow_lib/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:34:27.256926 chimpflow-1.4.1/src/chimpflow_lib/miners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 13:34:14.000000 chimpflow-1.4.1/src/chimpflow_lib/miners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-06-08 13:34:14.000000 chimpflow-1.4.1/src/chimpflow_lib/miners/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-08 13:34:14.000000 chimpflow-1.4.1/src/chimpflow_lib/miners/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-08 13:34:14.000000 chimpflow-1.4.1/src/chimpflow_lib/miners/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-06-08 13:34:14.000000 chimpflow-1.4.1/src/chimpflow_lib/miners/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-06-08 13:34:14.000000 chimpflow-1.4.1/src/chimpflow_lib/miners/direct_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-06-08 13:34:14.000000 chimpflow-1.4.1/src/chimpflow_lib/miners/miners.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-08 13:34:14.000000 chimpflow-1.4.1/src/chimpflow_lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:34:27.260926 chimpflow-1.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 13:34:14.000000 chimpflow-1.4.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-06-08 13:34:14.000000 chimpflow-1.4.1/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:34:27.260926 chimpflow-1.4.1/tests/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-08 13:34:14.000000 chimpflow-1.4.1/tests/configurations/direct_sqlite.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-08 13:34:14.000000 chimpflow-1.4.1/tests/configurations/service_mysql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-06-08 13:34:14.000000 chimpflow-1.4.1/tests/configurations/service_sqlite.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-06-08 13:34:14.000000 chimpflow-1.4.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:34:27.260926 chimpflow-1.4.1/tests/echo_test_imgs/
+-rw-r--r--   0 runner    (1001) docker     (123)   156218 2023-06-08 13:34:14.000000 chimpflow-1.4.1/tests/echo_test_imgs/97wo_01A_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   146361 2023-06-08 13:34:14.000000 chimpflow-1.4.1/tests/echo_test_imgs/97wo_01A_2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   142418 2023-06-08 13:34:14.000000 chimpflow-1.4.1/tests/echo_test_imgs/97wo_01A_3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-06-08 13:34:14.000000 chimpflow-1.4.1/tests/test_chimp_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-06-08 13:34:14.000000 chimpflow-1.4.1/tests/test_miner.py
```

### Comparing `chimpflow-1.4.0/.dae-devops/Makefile` & `chimpflow-1.4.1/.dae-devops/Makefile`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/.dae-devops/docs/conventions.rst` & `chimpflow-1.4.1/.dae-devops/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/.dae-devops/docs/developing.rst` & `chimpflow-1.4.1/.dae-devops/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/.dae-devops/docs/devops.rst` & `chimpflow-1.4.1/.dae-devops/docs/devops.rst`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/.dae-devops/docs/docs_structure.rst` & `chimpflow-1.4.1/.dae-devops/docs/docs_structure.rst`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/.dae-devops/docs/documenting.rst` & `chimpflow-1.4.1/.dae-devops/docs/documenting.rst`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/.dae-devops/docs/installing.rst` & `chimpflow-1.4.1/.dae-devops/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/.dae-devops/docs/testing.rst` & `chimpflow-1.4.1/.dae-devops/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/.dae-devops/project.yaml` & `chimpflow-1.4.1/.dae-devops/project.yaml`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/.devcontainer/Dockerfile` & `chimpflow-1.4.1/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/.devcontainer/devcontainer.json` & `chimpflow-1.4.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/.github/CONTRIBUTING.rst` & `chimpflow-1.4.1/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/.github/actions/install_requirements/action.yml` & `chimpflow-1.4.1/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/.github/dependabot.yml` & `chimpflow-1.4.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/.github/pages/make_switcher.py` & `chimpflow-1.4.1/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/.github/workflows/code.yml` & `chimpflow-1.4.1/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/.github/workflows/docs.yml` & `chimpflow-1.4.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/.github/workflows/docs_clean.yml` & `chimpflow-1.4.1/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/.github/workflows/linkcheck.yml` & `chimpflow-1.4.1/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/.gitignore` & `chimpflow-1.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/.gitlab-ci.yml` & `chimpflow-1.4.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/.vscode/launch.json` & `chimpflow-1.4.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/LICENSE` & `chimpflow-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/PKG-INFO` & `chimpflow-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chimpflow
-Version: 1.4.0
+Version: 1.4.1
 Summary: Service which polls the database for subwell images which need to have the chimp detector run on them.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `chimpflow-1.4.0/README.md` & `chimpflow-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/configurations/development.yaml` & `chimpflow-1.4.1/configurations/development.yaml`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/docs/conf.py` & `chimpflow-1.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/docs/images/dls-favicon.ico` & `chimpflow-1.4.1/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/docs/images/dls-logo.svg` & `chimpflow-1.4.1/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/pyproject.toml` & `chimpflow-1.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/src/chimpflow.egg-info/PKG-INFO` & `chimpflow-1.4.1/src/chimpflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chimpflow
-Version: 1.4.0
+Version: 1.4.1
 Summary: Service which polls the database for subwell images which need to have the chimp detector run on them.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `chimpflow-1.4.0/src/chimpflow.egg-info/SOURCES.txt` & `chimpflow-1.4.1/src/chimpflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/src/chimpflow_api/exceptions.py` & `chimpflow-1.4.1/src/chimpflow_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/src/chimpflow_api/miners/aiohttp.py` & `chimpflow-1.4.1/src/chimpflow_api/miners/aiohttp.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/src/chimpflow_api/miners/context.py` & `chimpflow-1.4.1/src/chimpflow_api/miners/context.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/src/chimpflow_api/miners/miners.py` & `chimpflow-1.4.1/src/chimpflow_api/miners/miners.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/src/chimpflow_api/thing.py` & `chimpflow-1.4.1/src/chimpflow_api/thing.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/src/chimpflow_api/things.py` & `chimpflow-1.4.1/src/chimpflow_api/things.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/src/chimpflow_cli/main.py` & `chimpflow-1.4.1/src/chimpflow_cli/main.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/src/chimpflow_cli/subcommands/base.py` & `chimpflow-1.4.1/src/chimpflow_cli/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/src/chimpflow_cli/subcommands/service.py` & `chimpflow-1.4.1/src/chimpflow_cli/subcommands/service.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/src/chimpflow_cli/version.py` & `chimpflow-1.4.1/src/chimpflow_cli/version.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/src/chimpflow_lib/__main__.py` & `chimpflow-1.4.1/src/chimpflow_lib/__main__.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/src/chimpflow_lib/chimp_adapter.py` & `chimpflow-1.4.1/src/chimpflow_lib/chimp_adapter.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/src/chimpflow_lib/exceptions.py` & `chimpflow-1.4.1/src/chimpflow_lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/src/chimpflow_lib/miners/aiohttp.py` & `chimpflow-1.4.1/src/chimpflow_lib/miners/aiohttp.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/src/chimpflow_lib/miners/base.py` & `chimpflow-1.4.1/src/chimpflow_lib/miners/base.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/src/chimpflow_lib/miners/context.py` & `chimpflow-1.4.1/src/chimpflow_lib/miners/context.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,24 +58,29 @@
 
         # Not running as a service?
         elif self.context_specification.get("start_as") == "direct":
             # We need to activate the tick() task.
             await self.server.activate()
 
     # ----------------------------------------------------------------------------------------
-    async def aexit(self, type, value, traceback) -> None:
+    async def aexit(self, type=None, value=None, traceback=None):
         """
         Asyncio context exit.
 
         Stop service if one was started and releases any client resources.
         """
 
+        logger.debug(f"[DISSHU] {thing_type} aexit")
+
         if self.server is not None:
             if self.context_specification.get("start_as") == "process":
-                # Put in request to shutdown the server.
-                await self.server.client_shutdown()
+                # The server associated with this context is running?
+                if await self.is_process_alive():
+                    logger.debug(f"[DISSHU] {thing_type} calling client_shutdown")
+                    # Put in request to shutdown the server.
+                    await self.server.client_shutdown()
 
             if self.context_specification.get("start_as") == "coro":
                 await self.server.direct_shutdown()
 
             if self.context_specification.get("start_as") == "direct":
                 await self.server.deactivate()
```

### Comparing `chimpflow-1.4.0/src/chimpflow_lib/miners/direct_poll.py` & `chimpflow-1.4.1/src/chimpflow_lib/miners/direct_poll.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/src/chimpflow_lib/miners/miners.py` & `chimpflow-1.4.1/src/chimpflow_lib/miners/miners.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/src/chimpflow_lib/version.py` & `chimpflow-1.4.1/src/chimpflow_lib/version.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/tests/base.py` & `chimpflow-1.4.1/tests/base.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/tests/configurations/direct_sqlite.yaml` & `chimpflow-1.4.1/tests/configurations/direct_sqlite.yaml`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/tests/configurations/service_mysql.yaml` & `chimpflow-1.4.1/tests/configurations/service_mysql.yaml`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/tests/configurations/service_sqlite.yaml` & `chimpflow-1.4.1/tests/configurations/service_sqlite.yaml`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/tests/conftest.py` & `chimpflow-1.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/tests/echo_test_imgs/97wo_01A_1.jpg` & `chimpflow-1.4.1/tests/echo_test_imgs/97wo_01A_1.jpg`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/tests/echo_test_imgs/97wo_01A_2.jpg` & `chimpflow-1.4.1/tests/echo_test_imgs/97wo_01A_2.jpg`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/tests/echo_test_imgs/97wo_01A_3.jpg` & `chimpflow-1.4.1/tests/echo_test_imgs/97wo_01A_3.jpg`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/tests/test_chimp_adapter.py` & `chimpflow-1.4.1/tests/test_chimp_adapter.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.4.0/tests/test_miner.py` & `chimpflow-1.4.1/tests/test_miner.py`

 * *Files identical despite different names*

