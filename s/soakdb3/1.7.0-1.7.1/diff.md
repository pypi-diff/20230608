# Comparing `tmp/soakdb3-1.7.0.tar.gz` & `tmp/soakdb3-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soakdb3-1.7.0.tar", last modified: Fri May 26 10:20:52 2023, max compression
+gzip compressed data, was "soakdb3-1.7.1.tar", last modified: Thu Jun  8 12:04:24 2023, max compression
```

## Comparing `soakdb3-1.7.0.tar` & `soakdb3-1.7.1.tar`

### file list

```diff
@@ -1,157 +1,158 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:20:52.076006 soakdb3-1.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:20:52.056006 soakdb3-1.7.0/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-05-26 10:20:41.000000 soakdb3-1.7.0/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:20:52.056006 soakdb3-1.7.0/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-26 10:20:41.000000 soakdb3-1.7.0/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-26 10:20:41.000000 soakdb3-1.7.0/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-26 10:20:41.000000 soakdb3-1.7.0/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-26 10:20:41.000000 soakdb3-1.7.0/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-26 10:20:41.000000 soakdb3-1.7.0/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-26 10:20:41.000000 soakdb3-1.7.0/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-26 10:20:41.000000 soakdb3-1.7.0/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-26 10:20:41.000000 soakdb3-1.7.0/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:20:52.056006 soakdb3-1.7.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-26 10:20:41.000000 soakdb3-1.7.0/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-05-26 10:20:41.000000 soakdb3-1.7.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:20:52.056006 soakdb3-1.7.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-26 10:20:41.000000 soakdb3-1.7.0/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:20:52.052005 soakdb3-1.7.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:20:52.056006 soakdb3-1.7.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-26 10:20:41.000000 soakdb3-1.7.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-26 10:20:41.000000 soakdb3-1.7.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:20:52.056006 soakdb3-1.7.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-26 10:20:41.000000 soakdb3-1.7.0/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-26 10:20:41.000000 soakdb3-1.7.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:20:52.056006 soakdb3-1.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     7071 2023-05-26 10:20:41.000000 soakdb3-1.7.0/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-26 10:20:41.000000 soakdb3-1.7.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-26 10:20:41.000000 soakdb3-1.7.0/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-26 10:20:41.000000 soakdb3-1.7.0/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-26 10:20:41.000000 soakdb3-1.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-05-26 10:20:41.000000 soakdb3-1.7.0/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-26 10:20:41.000000 soakdb3-1.7.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:20:52.056006 soakdb3-1.7.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-26 10:20:41.000000 soakdb3-1.7.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-26 10:20:41.000000 soakdb3-1.7.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-26 10:20:41.000000 soakdb3-1.7.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-26 10:20:41.000000 soakdb3-1.7.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-26 10:20:41.000000 soakdb3-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15806 2023-05-26 10:20:52.076006 soakdb3-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-05-26 10:20:41.000000 soakdb3-1.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:20:52.056006 soakdb3-1.7.0/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-26 10:20:41.000000 soakdb3-1.7.0/configurations/development.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:20:52.060006 soakdb3-1.7.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:20:52.052005 soakdb3-1.7.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:20:52.060006 soakdb3-1.7.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-26 10:20:41.000000 soakdb3-1.7.0/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     6693 2023-05-26 10:20:41.000000 soakdb3-1.7.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:20:52.060006 soakdb3-1.7.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)   305758 2023-05-26 10:20:41.000000 soakdb3-1.7.0/docs/images/Office 365 error.png
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-26 10:20:41.000000 soakdb3-1.7.0/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-26 10:20:41.000000 soakdb3-1.7.0/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-26 10:20:41.000000 soakdb3-1.7.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:20:52.060006 soakdb3-1.7.0/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:20:52.060006 soakdb3-1.7.0/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-26 10:20:41.000000 soakdb3-1.7.0/docs/user/explanations/22-developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-26 10:20:41.000000 soakdb3-1.7.0/docs/user/explanations/23-testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-26 10:20:41.000000 soakdb3-1.7.0/docs/user/explanations/24-devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-26 10:20:41.000000 soakdb3-1.7.0/docs/user/explanations/25-docs-structure.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:20:52.060006 soakdb3-1.7.0/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-26 10:20:41.000000 soakdb3-1.7.0/docs/user/how-to/01-installing_development.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-26 10:20:41.000000 soakdb3-1.7.0/docs/user/how-to/03-starting_development.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-05-26 10:20:41.000000 soakdb3-1.7.0/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:20:52.060006 soakdb3-1.7.0/docs/user/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-26 10:20:41.000000 soakdb3-1.7.0/docs/user/reference/01-conda.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:20:52.060006 soakdb3-1.7.0/docs/user/reference/api/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-26 10:20:41.000000 soakdb3-1.7.0/docs/user/reference/api/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-26 10:20:41.000000 soakdb3-1.7.0/docs/user/reference/api/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-26 10:20:41.000000 soakdb3-1.7.0/docs/user/reference/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-26 10:20:41.000000 soakdb3-1.7.0/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:20:52.060006 soakdb3-1.7.0/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-26 10:20:41.000000 soakdb3-1.7.0/docs/user/tutorials/02-starting_backend.rst
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-26 10:20:41.000000 soakdb3-1.7.0/docs/user/tutorials/03-starting_frontend.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:20:52.052005 soakdb3-1.7.0/docs/user/tutorials/images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:20:52.060006 soakdb3-1.7.0/docs/user/tutorials/images/submitting_gui/
--rw-r--r--   0 runner    (1001) docker     (123)    55338 2023-05-26 10:20:41.000000 soakdb3-1.7.0/docs/user/tutorials/images/submitting_gui/finish.png
--rw-r--r--   0 runner    (1001) docker     (123)    43233 2023-05-26 10:20:41.000000 soakdb3-1.7.0/docs/user/tutorials/images/submitting_gui/post_submit.png
--rw-r--r--   0 runner    (1001) docker     (123)    24403 2023-05-26 10:20:41.000000 soakdb3-1.7.0/docs/user/tutorials/images/submitting_gui/pre_submit.png
--rw-r--r--   0 runner    (1001) docker     (123)    23173 2023-05-26 10:20:41.000000 soakdb3-1.7.0/docs/user/tutorials/images/submitting_gui/start.png
--rw-r--r--   0 runner    (1001) docker     (123)    54940 2023-05-26 10:20:41.000000 soakdb3-1.7.0/docs/user/tutorials/images/submitting_gui/stdout.png
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-26 10:20:41.000000 soakdb3-1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 10:20:52.076006 soakdb3-1.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:20:52.052005 soakdb3-1.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:20:52.064006 soakdb3-1.7.0/src/soakdb3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15806 2023-05-26 10:20:51.000000 soakdb3-1.7.0/src/soakdb3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-26 10:20:52.000000 soakdb3-1.7.0/src/soakdb3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 10:20:51.000000 soakdb3-1.7.0/src/soakdb3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-26 10:20:51.000000 soakdb3-1.7.0/src/soakdb3.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-26 10:20:51.000000 soakdb3-1.7.0/src/soakdb3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-26 10:20:51.000000 soakdb3-1.7.0/src/soakdb3.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:20:52.064006 soakdb3-1.7.0/src/soakdb3_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:20:41.000000 soakdb3-1.7.0/src/soakdb3_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-26 10:20:41.000000 soakdb3-1.7.0/src/soakdb3_api/aiohttp_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:20:52.064006 soakdb3-1.7.0/src/soakdb3_api/databases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:20:41.000000 soakdb3-1.7.0/src/soakdb3_api/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-26 10:20:41.000000 soakdb3-1.7.0/src/soakdb3_api/databases/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-26 10:20:41.000000 soakdb3-1.7.0/src/soakdb3_api/databases/database_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     6058 2023-05-26 10:20:41.000000 soakdb3-1.7.0/src/soakdb3_api/databases/table_definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:20:52.064006 soakdb3-1.7.0/src/soakdb3_api/datafaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:20:41.000000 soakdb3-1.7.0/src/soakdb3_api/datafaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-05-26 10:20:41.000000 soakdb3-1.7.0/src/soakdb3_api/datafaces/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-26 10:20:41.000000 soakdb3-1.7.0/src/soakdb3_api/datafaces/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-26 10:20:41.000000 soakdb3-1.7.0/src/soakdb3_api/datafaces/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-26 10:20:41.000000 soakdb3-1.7.0/src/soakdb3_api/datafaces/datafaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-26 10:20:41.000000 soakdb3-1.7.0/src/soakdb3_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:20:52.064006 soakdb3-1.7.0/src/soakdb3_api/models/
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-26 10:20:41.000000 soakdb3-1.7.0/src/soakdb3_api/models/crystal_well_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:20:52.064006 soakdb3-1.7.0/src/soakdb3_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:20:41.000000 soakdb3-1.7.0/src/soakdb3_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:20:52.052005 soakdb3-1.7.0/src/soakdb3_cli/configurations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:20:52.064006 soakdb3-1.7.0/src/soakdb3_cli/configurations/default/
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-26 10:20:41.000000 soakdb3-1.7.0/src/soakdb3_cli/configurations/default/configuration.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-05-26 10:20:41.000000 soakdb3-1.7.0/src/soakdb3_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:20:52.064006 soakdb3-1.7.0/src/soakdb3_cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:20:41.000000 soakdb3-1.7.0/src/soakdb3_cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-05-26 10:20:41.000000 soakdb3-1.7.0/src/soakdb3_cli/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-26 10:20:41.000000 soakdb3-1.7.0/src/soakdb3_cli/subcommands/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-26 10:20:41.000000 soakdb3-1.7.0/src/soakdb3_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:20:52.068006 soakdb3-1.7.0/src/soakdb3_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-26 10:20:41.000000 soakdb3-1.7.0/src/soakdb3_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-26 10:20:41.000000 soakdb3-1.7.0/src/soakdb3_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-26 10:20:51.000000 soakdb3-1.7.0/src/soakdb3_lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-26 10:20:41.000000 soakdb3-1.7.0/src/soakdb3_lib/base_aiohttp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:20:52.068006 soakdb3-1.7.0/src/soakdb3_lib/datafaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:20:41.000000 soakdb3-1.7.0/src/soakdb3_lib/datafaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-05-26 10:20:41.000000 soakdb3-1.7.0/src/soakdb3_lib/datafaces/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-05-26 10:20:41.000000 soakdb3-1.7.0/src/soakdb3_lib/datafaces/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-26 10:20:41.000000 soakdb3-1.7.0/src/soakdb3_lib/datafaces/datafaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    23052 2023-05-26 10:20:41.000000 soakdb3-1.7.0/src/soakdb3_lib/datafaces/normsql.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-26 10:20:41.000000 soakdb3-1.7.0/src/soakdb3_lib/envvar.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-26 10:20:41.000000 soakdb3-1.7.0/src/soakdb3_lib/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-26 10:20:41.000000 soakdb3-1.7.0/src/soakdb3_lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:20:52.068006 soakdb3-1.7.0/src/soakdb3_xls/
--rw-r--r--   0 runner    (1001) docker     (123)   407625 2023-05-26 10:20:41.000000 soakdb3-1.7.0/src/soakdb3_xls/XsoakDB_v3.0_library.xlsm
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:20:41.000000 soakdb3-1.7.0/src/soakdb3_xls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-26 10:20:41.000000 soakdb3-1.7.0/src/soakdb3_xls/excel_config.json
--rw-r--r--   0 runner    (1001) docker     (123)    21125 2023-05-26 10:20:41.000000 soakdb3-1.7.0/src/soakdb3_xls/import_export.xlsm
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-26 10:20:41.000000 soakdb3-1.7.0/src/soakdb3_xls/lb19758-64.bat
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-26 10:20:41.000000 soakdb3-1.7.0/src/soakdb3_xls/soakDB3.bat
--rw-r--r--   0 runner    (1001) docker     (123)  6166705 2023-05-26 10:20:41.000000 soakdb3-1.7.0/src/soakdb3_xls/soakDB_v3.0.xlsm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:20:52.076006 soakdb3-1.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:20:41.000000 soakdb3-1.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-26 10:20:41.000000 soakdb3-1.7.0/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-26 10:20:41.000000 soakdb3-1.7.0/tests/base_context_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-26 10:20:41.000000 soakdb3-1.7.0/tests/base_specification_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-26 10:20:41.000000 soakdb3-1.7.0/tests/base_tester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:20:52.076006 soakdb3-1.7.0/tests/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-26 10:20:41.000000 soakdb3-1.7.0/tests/configurations/filestore.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-05-26 10:20:41.000000 soakdb3-1.7.0/tests/configurations/services.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    27817 2023-05-26 10:20:41.000000 soakdb3-1.7.0/tests/configurations/store.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-05-26 10:20:41.000000 soakdb3-1.7.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-05-26 10:20:41.000000 soakdb3-1.7.0/tests/test_assign_pin_barcodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-05-26 10:20:41.000000 soakdb3-1.7.0/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-05-26 10:20:41.000000 soakdb3-1.7.0/tests/test_database_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-05-26 10:20:41.000000 soakdb3-1.7.0/tests/test_database_revision.py
--rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-05-26 10:20:41.000000 soakdb3-1.7.0/tests/test_dataface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-05-26 10:20:41.000000 soakdb3-1.7.0/tests/test_move_to_done.py
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-05-26 10:20:41.000000 soakdb3-1.7.0/tests/test_write_csv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:04:24.185617 soakdb3-1.7.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:04:24.153617 soakdb3-1.7.1/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-08 12:04:09.000000 soakdb3-1.7.1/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:04:24.157617 soakdb3-1.7.1/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-08 12:04:09.000000 soakdb3-1.7.1/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-08 12:04:09.000000 soakdb3-1.7.1/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-08 12:04:09.000000 soakdb3-1.7.1/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-08 12:04:09.000000 soakdb3-1.7.1/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-08 12:04:09.000000 soakdb3-1.7.1/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-08 12:04:09.000000 soakdb3-1.7.1/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-08 12:04:09.000000 soakdb3-1.7.1/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-08 12:04:09.000000 soakdb3-1.7.1/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:04:24.157617 soakdb3-1.7.1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-08 12:04:09.000000 soakdb3-1.7.1/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-08 12:04:09.000000 soakdb3-1.7.1/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:04:24.157617 soakdb3-1.7.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-08 12:04:09.000000 soakdb3-1.7.1/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:04:24.149617 soakdb3-1.7.1/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:04:24.157617 soakdb3-1.7.1/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-06-08 12:04:09.000000 soakdb3-1.7.1/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-08 12:04:09.000000 soakdb3-1.7.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:04:24.157617 soakdb3-1.7.1/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-08 12:04:09.000000 soakdb3-1.7.1/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-06-08 12:04:09.000000 soakdb3-1.7.1/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:04:24.157617 soakdb3-1.7.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     7071 2023-06-08 12:04:09.000000 soakdb3-1.7.1/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-06-08 12:04:09.000000 soakdb3-1.7.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-08 12:04:09.000000 soakdb3-1.7.1/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-08 12:04:09.000000 soakdb3-1.7.1/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-08 12:04:09.000000 soakdb3-1.7.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-06-08 12:04:09.000000 soakdb3-1.7.1/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-08 12:04:09.000000 soakdb3-1.7.1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:04:24.157617 soakdb3-1.7.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-08 12:04:09.000000 soakdb3-1.7.1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-08 12:04:09.000000 soakdb3-1.7.1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-08 12:04:09.000000 soakdb3-1.7.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-08 12:04:09.000000 soakdb3-1.7.1/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-08 12:04:09.000000 soakdb3-1.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15806 2023-06-08 12:04:24.185617 soakdb3-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-06-08 12:04:09.000000 soakdb3-1.7.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:04:24.157617 soakdb3-1.7.1/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-08 12:04:09.000000 soakdb3-1.7.1/configurations/development.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:04:24.157617 soakdb3-1.7.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:04:24.149617 soakdb3-1.7.1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:04:24.161617 soakdb3-1.7.1/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-08 12:04:09.000000 soakdb3-1.7.1/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6693 2023-06-08 12:04:09.000000 soakdb3-1.7.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:04:24.161617 soakdb3-1.7.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   305758 2023-06-08 12:04:09.000000 soakdb3-1.7.1/docs/images/Office 365 error.png
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-06-08 12:04:09.000000 soakdb3-1.7.1/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-08 12:04:09.000000 soakdb3-1.7.1/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-08 12:04:09.000000 soakdb3-1.7.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:04:24.161617 soakdb3-1.7.1/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:04:24.161617 soakdb3-1.7.1/docs/user/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-08 12:04:09.000000 soakdb3-1.7.1/docs/user/explanations/22-developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-08 12:04:09.000000 soakdb3-1.7.1/docs/user/explanations/23-testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-08 12:04:09.000000 soakdb3-1.7.1/docs/user/explanations/24-devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-08 12:04:09.000000 soakdb3-1.7.1/docs/user/explanations/25-docs-structure.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:04:24.161617 soakdb3-1.7.1/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-08 12:04:09.000000 soakdb3-1.7.1/docs/user/how-to/01-installing_development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-08 12:04:09.000000 soakdb3-1.7.1/docs/user/how-to/03-starting_development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-08 12:04:09.000000 soakdb3-1.7.1/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:04:24.161617 soakdb3-1.7.1/docs/user/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-08 12:04:09.000000 soakdb3-1.7.1/docs/user/reference/01-conda.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:04:24.161617 soakdb3-1.7.1/docs/user/reference/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-08 12:04:09.000000 soakdb3-1.7.1/docs/user/reference/api/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-08 12:04:09.000000 soakdb3-1.7.1/docs/user/reference/api/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-08 12:04:09.000000 soakdb3-1.7.1/docs/user/reference/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-08 12:04:09.000000 soakdb3-1.7.1/docs/user/reference/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:04:24.161617 soakdb3-1.7.1/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-08 12:04:09.000000 soakdb3-1.7.1/docs/user/tutorials/02-starting_backend.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-08 12:04:09.000000 soakdb3-1.7.1/docs/user/tutorials/03-starting_frontend.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:04:24.153617 soakdb3-1.7.1/docs/user/tutorials/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:04:24.165617 soakdb3-1.7.1/docs/user/tutorials/images/submitting_gui/
+-rw-r--r--   0 runner    (1001) docker     (123)    55338 2023-06-08 12:04:09.000000 soakdb3-1.7.1/docs/user/tutorials/images/submitting_gui/finish.png
+-rw-r--r--   0 runner    (1001) docker     (123)    43233 2023-06-08 12:04:09.000000 soakdb3-1.7.1/docs/user/tutorials/images/submitting_gui/post_submit.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24403 2023-06-08 12:04:09.000000 soakdb3-1.7.1/docs/user/tutorials/images/submitting_gui/pre_submit.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23173 2023-06-08 12:04:09.000000 soakdb3-1.7.1/docs/user/tutorials/images/submitting_gui/start.png
+-rw-r--r--   0 runner    (1001) docker     (123)    54940 2023-06-08 12:04:09.000000 soakdb3-1.7.1/docs/user/tutorials/images/submitting_gui/stdout.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-08 12:04:09.000000 soakdb3-1.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 12:04:24.185617 soakdb3-1.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:04:24.153617 soakdb3-1.7.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:04:24.165617 soakdb3-1.7.1/src/soakdb3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15806 2023-06-08 12:04:24.000000 soakdb3-1.7.1/src/soakdb3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-06-08 12:04:24.000000 soakdb3-1.7.1/src/soakdb3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 12:04:24.000000 soakdb3-1.7.1/src/soakdb3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-08 12:04:24.000000 soakdb3-1.7.1/src/soakdb3.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-08 12:04:24.000000 soakdb3-1.7.1/src/soakdb3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-08 12:04:24.000000 soakdb3-1.7.1/src/soakdb3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:04:24.165617 soakdb3-1.7.1/src/soakdb3_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:04:09.000000 soakdb3-1.7.1/src/soakdb3_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-08 12:04:09.000000 soakdb3-1.7.1/src/soakdb3_api/aiohttp_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:04:24.165617 soakdb3-1.7.1/src/soakdb3_api/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:04:09.000000 soakdb3-1.7.1/src/soakdb3_api/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-06-08 12:04:09.000000 soakdb3-1.7.1/src/soakdb3_api/databases/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-08 12:04:09.000000 soakdb3-1.7.1/src/soakdb3_api/databases/database_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6058 2023-06-08 12:04:09.000000 soakdb3-1.7.1/src/soakdb3_api/databases/table_definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:04:24.169617 soakdb3-1.7.1/src/soakdb3_api/datafaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:04:09.000000 soakdb3-1.7.1/src/soakdb3_api/datafaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-06-08 12:04:09.000000 soakdb3-1.7.1/src/soakdb3_api/datafaces/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-08 12:04:09.000000 soakdb3-1.7.1/src/soakdb3_api/datafaces/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-06-08 12:04:09.000000 soakdb3-1.7.1/src/soakdb3_api/datafaces/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-06-08 12:04:09.000000 soakdb3-1.7.1/src/soakdb3_api/datafaces/datafaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-08 12:04:09.000000 soakdb3-1.7.1/src/soakdb3_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:04:24.169617 soakdb3-1.7.1/src/soakdb3_api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-08 12:04:09.000000 soakdb3-1.7.1/src/soakdb3_api/models/crystal_well_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-08 12:04:09.000000 soakdb3-1.7.1/src/soakdb3_api/xce_shim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:04:24.169617 soakdb3-1.7.1/src/soakdb3_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:04:09.000000 soakdb3-1.7.1/src/soakdb3_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:04:24.153617 soakdb3-1.7.1/src/soakdb3_cli/configurations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:04:24.169617 soakdb3-1.7.1/src/soakdb3_cli/configurations/default/
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-08 12:04:09.000000 soakdb3-1.7.1/src/soakdb3_cli/configurations/default/configuration.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-06-08 12:04:09.000000 soakdb3-1.7.1/src/soakdb3_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:04:24.169617 soakdb3-1.7.1/src/soakdb3_cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:04:09.000000 soakdb3-1.7.1/src/soakdb3_cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-06-08 12:04:09.000000 soakdb3-1.7.1/src/soakdb3_cli/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-08 12:04:09.000000 soakdb3-1.7.1/src/soakdb3_cli/subcommands/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-08 12:04:09.000000 soakdb3-1.7.1/src/soakdb3_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:04:24.169617 soakdb3-1.7.1/src/soakdb3_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-08 12:04:09.000000 soakdb3-1.7.1/src/soakdb3_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-08 12:04:09.000000 soakdb3-1.7.1/src/soakdb3_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-08 12:04:23.000000 soakdb3-1.7.1/src/soakdb3_lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-08 12:04:09.000000 soakdb3-1.7.1/src/soakdb3_lib/base_aiohttp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:04:24.173617 soakdb3-1.7.1/src/soakdb3_lib/datafaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:04:09.000000 soakdb3-1.7.1/src/soakdb3_lib/datafaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-06-08 12:04:09.000000 soakdb3-1.7.1/src/soakdb3_lib/datafaces/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-08 12:04:09.000000 soakdb3-1.7.1/src/soakdb3_lib/datafaces/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-08 12:04:09.000000 soakdb3-1.7.1/src/soakdb3_lib/datafaces/datafaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23052 2023-06-08 12:04:09.000000 soakdb3-1.7.1/src/soakdb3_lib/datafaces/normsql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-08 12:04:09.000000 soakdb3-1.7.1/src/soakdb3_lib/envvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-08 12:04:09.000000 soakdb3-1.7.1/src/soakdb3_lib/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-08 12:04:09.000000 soakdb3-1.7.1/src/soakdb3_lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:04:24.173617 soakdb3-1.7.1/src/soakdb3_xls/
+-rw-r--r--   0 runner    (1001) docker     (123)   407625 2023-06-08 12:04:09.000000 soakdb3-1.7.1/src/soakdb3_xls/XsoakDB_v3.0_library.xlsm
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:04:09.000000 soakdb3-1.7.1/src/soakdb3_xls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-08 12:04:09.000000 soakdb3-1.7.1/src/soakdb3_xls/excel_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21125 2023-06-08 12:04:09.000000 soakdb3-1.7.1/src/soakdb3_xls/import_export.xlsm
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-08 12:04:09.000000 soakdb3-1.7.1/src/soakdb3_xls/lb19758-64.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-08 12:04:09.000000 soakdb3-1.7.1/src/soakdb3_xls/soakDB3.bat
+-rw-r--r--   0 runner    (1001) docker     (123)  6166705 2023-06-08 12:04:09.000000 soakdb3-1.7.1/src/soakdb3_xls/soakDB_v3.0.xlsm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:04:24.185617 soakdb3-1.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:04:09.000000 soakdb3-1.7.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-08 12:04:09.000000 soakdb3-1.7.1/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-08 12:04:09.000000 soakdb3-1.7.1/tests/base_context_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-08 12:04:09.000000 soakdb3-1.7.1/tests/base_specification_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-08 12:04:09.000000 soakdb3-1.7.1/tests/base_tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:04:24.185617 soakdb3-1.7.1/tests/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-08 12:04:09.000000 soakdb3-1.7.1/tests/configurations/filestore.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-06-08 12:04:09.000000 soakdb3-1.7.1/tests/configurations/services.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    27817 2023-06-08 12:04:09.000000 soakdb3-1.7.1/tests/configurations/store.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-06-08 12:04:09.000000 soakdb3-1.7.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-06-08 12:04:09.000000 soakdb3-1.7.1/tests/test_assign_pin_barcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-06-08 12:04:09.000000 soakdb3-1.7.1/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-06-08 12:04:09.000000 soakdb3-1.7.1/tests/test_database_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-08 12:04:09.000000 soakdb3-1.7.1/tests/test_database_revision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-06-08 12:04:09.000000 soakdb3-1.7.1/tests/test_dataface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-06-08 12:04:09.000000 soakdb3-1.7.1/tests/test_move_to_done.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-06-08 12:04:09.000000 soakdb3-1.7.1/tests/test_write_csv.py
```

### Comparing `soakdb3-1.7.0/.dae-devops/Makefile` & `soakdb3-1.7.1/.dae-devops/Makefile`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/.dae-devops/docs/conventions.rst` & `soakdb3-1.7.1/.dae-devops/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/.dae-devops/docs/developing.rst` & `soakdb3-1.7.1/.dae-devops/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/.dae-devops/docs/devops.rst` & `soakdb3-1.7.1/.dae-devops/docs/devops.rst`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/.dae-devops/docs/docs_structure.rst` & `soakdb3-1.7.1/.dae-devops/docs/docs_structure.rst`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/.dae-devops/docs/installing.rst` & `soakdb3-1.7.1/.dae-devops/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/.dae-devops/docs/testing.rst` & `soakdb3-1.7.1/.dae-devops/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/.dae-devops/project.yaml` & `soakdb3-1.7.1/.dae-devops/project.yaml`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/.devcontainer/Dockerfile` & `soakdb3-1.7.1/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/.devcontainer/devcontainer.json` & `soakdb3-1.7.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/.github/CONTRIBUTING.rst` & `soakdb3-1.7.1/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/.github/actions/install_requirements/action.yml` & `soakdb3-1.7.1/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/.github/dependabot.yml` & `soakdb3-1.7.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/.github/pages/make_switcher.py` & `soakdb3-1.7.1/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/.github/workflows/code.yml` & `soakdb3-1.7.1/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/.github/workflows/docs.yml` & `soakdb3-1.7.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/.github/workflows/docs_clean.yml` & `soakdb3-1.7.1/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/.github/workflows/linkcheck.yml` & `soakdb3-1.7.1/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/.gitignore` & `soakdb3-1.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/.gitlab-ci.yml` & `soakdb3-1.7.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/.vscode/launch.json` & `soakdb3-1.7.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/LICENSE` & `soakdb3-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/PKG-INFO` & `soakdb3-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soakdb3
-Version: 1.7.0
+Version: 1.7.1
 Summary: Replacement for soakdb2, including a new database backend.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `soakdb3-1.7.0/README.rst` & `soakdb3-1.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/configurations/development.yaml` & `soakdb3-1.7.1/configurations/development.yaml`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/docs/conf.py` & `soakdb3-1.7.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/docs/images/Office 365 error.png` & `soakdb3-1.7.1/docs/images/Office 365 error.png`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/docs/images/dls-favicon.ico` & `soakdb3-1.7.1/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/docs/images/dls-logo.svg` & `soakdb3-1.7.1/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/docs/index.rst` & `soakdb3-1.7.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/docs/user/explanations/25-docs-structure.rst` & `soakdb3-1.7.1/docs/user/explanations/25-docs-structure.rst`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/docs/user/how-to/03-starting_development.rst` & `soakdb3-1.7.1/docs/user/how-to/03-starting_development.rst`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/docs/user/index.rst` & `soakdb3-1.7.1/docs/user/index.rst`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/docs/user/reference/01-conda.rst` & `soakdb3-1.7.1/docs/user/reference/01-conda.rst`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/docs/user/tutorials/02-starting_backend.rst` & `soakdb3-1.7.1/docs/user/tutorials/02-starting_backend.rst`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/docs/user/tutorials/03-starting_frontend.rst` & `soakdb3-1.7.1/docs/user/tutorials/03-starting_frontend.rst`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/docs/user/tutorials/images/submitting_gui/finish.png` & `soakdb3-1.7.1/docs/user/tutorials/images/submitting_gui/finish.png`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/docs/user/tutorials/images/submitting_gui/post_submit.png` & `soakdb3-1.7.1/docs/user/tutorials/images/submitting_gui/post_submit.png`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/docs/user/tutorials/images/submitting_gui/pre_submit.png` & `soakdb3-1.7.1/docs/user/tutorials/images/submitting_gui/pre_submit.png`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/docs/user/tutorials/images/submitting_gui/start.png` & `soakdb3-1.7.1/docs/user/tutorials/images/submitting_gui/start.png`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/docs/user/tutorials/images/submitting_gui/stdout.png` & `soakdb3-1.7.1/docs/user/tutorials/images/submitting_gui/stdout.png`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/pyproject.toml` & `soakdb3-1.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/src/soakdb3.egg-info/PKG-INFO` & `soakdb3-1.7.1/src/soakdb3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soakdb3
-Version: 1.7.0
+Version: 1.7.1
 Summary: Replacement for soakdb2, including a new database backend.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `soakdb3-1.7.0/src/soakdb3.egg-info/SOURCES.txt` & `soakdb3-1.7.1/src/soakdb3.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 src/soakdb3.egg-info/dependency_links.txt
 src/soakdb3.egg-info/entry_points.txt
 src/soakdb3.egg-info/requires.txt
 src/soakdb3.egg-info/top_level.txt
 src/soakdb3_api/__init__.py
 src/soakdb3_api/aiohttp_client.py
 src/soakdb3_api/exceptions.py
+src/soakdb3_api/xce_shim.py
 src/soakdb3_api/databases/__init__.py
 src/soakdb3_api/databases/constants.py
 src/soakdb3_api/databases/database_definition.py
 src/soakdb3_api/databases/table_definitions.py
 src/soakdb3_api/datafaces/__init__.py
 src/soakdb3_api/datafaces/aiohttp.py
 src/soakdb3_api/datafaces/constants.py
```

### Comparing `soakdb3-1.7.0/src/soakdb3_api/databases/constants.py` & `soakdb3-1.7.1/src/soakdb3_api/databases/constants.py`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/src/soakdb3_api/databases/database_definition.py` & `soakdb3-1.7.1/src/soakdb3_api/databases/database_definition.py`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/src/soakdb3_api/databases/table_definitions.py` & `soakdb3-1.7.1/src/soakdb3_api/databases/table_definitions.py`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/src/soakdb3_api/datafaces/aiohttp.py` & `soakdb3-1.7.1/src/soakdb3_api/datafaces/aiohttp.py`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/src/soakdb3_api/datafaces/context.py` & `soakdb3-1.7.1/src/soakdb3_api/datafaces/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 class Context:
     """
     Client context for a dataface object.
     On entering, it creates the object according to the specification (a dict).
     On exiting, it closes client connection.
 
-    The aenter and aexit methods are exposed for use by an enclosing context.
+    The aenter and aexit methods are exposed for use by an enclosing context and the base class.
     """
 
     # ----------------------------------------------------------------------------------------
     def __init__(self, specification):
         self.__specification = specification
         self.__dataface = None
```

### Comparing `soakdb3-1.7.0/src/soakdb3_api/datafaces/datafaces.py` & `soakdb3-1.7.1/src/soakdb3_api/datafaces/datafaces.py`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/src/soakdb3_api/exceptions.py` & `soakdb3-1.7.1/src/soakdb3_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/src/soakdb3_api/models/crystal_well_model.py` & `soakdb3-1.7.1/src/soakdb3_api/models/crystal_well_model.py`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/src/soakdb3_cli/configurations/default/configuration.yaml` & `soakdb3-1.7.1/src/soakdb3_cli/configurations/default/configuration.yaml`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/src/soakdb3_cli/main.py` & `soakdb3-1.7.1/src/soakdb3_cli/main.py`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/src/soakdb3_cli/subcommands/base.py` & `soakdb3-1.7.1/src/soakdb3_cli/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/src/soakdb3_cli/subcommands/service.py` & `soakdb3-1.7.1/src/soakdb3_cli/subcommands/service.py`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/src/soakdb3_cli/version.py` & `soakdb3-1.7.1/src/soakdb3_cli/version.py`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/src/soakdb3_lib/__main__.py` & `soakdb3-1.7.1/src/soakdb3_lib/__main__.py`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/src/soakdb3_lib/datafaces/aiohttp.py` & `soakdb3-1.7.1/src/soakdb3_lib/datafaces/aiohttp.py`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/src/soakdb3_lib/datafaces/context.py` & `soakdb3-1.7.1/src/soakdb3_lib/datafaces/context.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,20 +47,28 @@
             await self.server.start_thread()
 
         elif self.context_specification.get("start_as") == "process":
             await self.server.start_process()
 
     # ----------------------------------------------------------------------------------------
     async def aexit(self):
-        """ """
+        """
+        Asyncio context exit.
+
+        Stop service if one was started and releases any client resources.
+        """
+        logger.debug(f"[DISSHU] {thing_type} aexit")
 
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
 
     # ----------------------------------------------------------------------------------------
     async def __aenter__(self):
         """ """
```

### Comparing `soakdb3-1.7.0/src/soakdb3_lib/datafaces/datafaces.py` & `soakdb3-1.7.1/src/soakdb3_lib/datafaces/datafaces.py`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/src/soakdb3_lib/datafaces/normsql.py` & `soakdb3-1.7.1/src/soakdb3_lib/datafaces/normsql.py`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/src/soakdb3_lib/envvar.py` & `soakdb3-1.7.1/src/soakdb3_lib/envvar.py`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/src/soakdb3_lib/version.py` & `soakdb3-1.7.1/src/soakdb3_lib/version.py`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/src/soakdb3_xls/XsoakDB_v3.0_library.xlsm` & `soakdb3-1.7.1/src/soakdb3_xls/XsoakDB_v3.0_library.xlsm`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/src/soakdb3_xls/import_export.xlsm` & `soakdb3-1.7.1/src/soakdb3_xls/import_export.xlsm`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/src/soakdb3_xls/soakDB_v3.0.xlsm` & `soakdb3-1.7.1/src/soakdb3_xls/soakDB_v3.0.xlsm`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/tests/base.py` & `soakdb3-1.7.1/tests/base.py`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/tests/base_context_tester.py` & `soakdb3-1.7.1/tests/base_context_tester.py`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/tests/base_specification_tester.py` & `soakdb3-1.7.1/tests/base_specification_tester.py`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/tests/base_tester.py` & `soakdb3-1.7.1/tests/base_tester.py`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/tests/configurations/filestore.yaml` & `soakdb3-1.7.1/tests/configurations/filestore.yaml`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/tests/configurations/services.yaml` & `soakdb3-1.7.1/tests/configurations/services.yaml`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/tests/configurations/store.csv` & `soakdb3-1.7.1/tests/configurations/store.csv`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/tests/conftest.py` & `soakdb3-1.7.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/tests/test_assign_pin_barcodes.py` & `soakdb3-1.7.1/tests/test_assign_pin_barcodes.py`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/tests/test_database.py` & `soakdb3-1.7.1/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/tests/test_database_backup.py` & `soakdb3-1.7.1/tests/test_database_backup.py`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/tests/test_database_revision.py` & `soakdb3-1.7.1/tests/test_database_revision.py`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/tests/test_dataface.py` & `soakdb3-1.7.1/tests/test_dataface.py`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/tests/test_move_to_done.py` & `soakdb3-1.7.1/tests/test_move_to_done.py`

 * *Files identical despite different names*

### Comparing `soakdb3-1.7.0/tests/test_write_csv.py` & `soakdb3-1.7.1/tests/test_write_csv.py`

 * *Files identical despite different names*

